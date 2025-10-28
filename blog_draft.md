# ✨ Fine-Tuning Three Transformer Architectures for NLP Tasks

In **Project 02**, I fine-tuned three different Transformer models — 
**BERT**, **GPT-2**, and **T5** — each representing a major architecture type:
Encoder-only, Decoder-only, and Encoder–Decoder.

The goal was to explore how each model performs on different kinds of NLP tasks:
classification, generation, and summarization.

---

## 🧠 Task 1 — BERT for Emotion Detection
**Dataset:** [Kaggle — Emotion Categories](https://www.kaggle.com/datasets/faiqahmad01/emotion-categories-neutraljoysadnessanger)

**Objective:** Classify text into Neutral, Joy, Sadness, or Anger.  
**Model:** `bert-base-cased`

**Training Setup**
- Optimizer: Adam (lr=5e-5)
- Epochs: 3
- Loss: SparseCategoricalCrossEntropy
- Trained on: Colab T4 GPU

**Results**
- Accuracy: 0.611  
- Macro F1: 0.615  
- Weighted F1: 0.617  

**Key Insight:**  
BERT captured contextual emotion cues effectively, performing best on *Joy* and *Anger* but confusing *Sadness* vs *Neutral* due to tone overlap.

---

## 🍳 Task 2 — GPT-2 for Recipe Generation
**Dataset:** [3A2M Extended Recipe Dataset](https://www.kaggle.com/datasets/nazmussakibrupol/3a2mext/data)

**Objective:** Generate coherent cooking recipes from dish names or ingredient lists.  
**Model:** `gpt2`

**Training:**  
- 3 epochs, lr=5e-5  
- Tokenizer: GPT-2 with EOS token as padding

**Evaluation:**
- ROUGE-1 = 0.24, ROUGE-L = 0.14, BLEU = 0.013

**Observation:**  
Generated recipes were realistic and contextually relevant, demonstrating GPT-2’s creative text-generation strength.

---

## 📰 Task 3 — T5 for Text Summarization
**Dataset:** [CNN/DailyMail Summarization Dataset](https://www.kaggle.com/datasets/gowrishankarp/newspaper-text-summarization-cnn-dailymail)

**Objective:** Generate concise summaries from long news articles.  
**Model:** `t5-small`

**Results:**
- ROUGE-1 = 10.63  
- ROUGE-2 = 1.83  
- ROUGE-L = 9.48  

**Insights:**  
T5 successfully produced short summaries that retained main context. 
Training with a larger model (T5-Base) and more epochs could further improve quality.

---

## 🚀 Takeaways
| Architecture | Strength | Use-Case Example |
|--------------|-----------|------------------|
| Encoder-only | Deep semantic understanding | Emotion Detection |
| Decoder-only | Creative text generation | Recipe Generation |
| Encoder-Decoder | Balanced understanding + generation | Summarization |

Working across these architectures revealed how model design aligns with task type and data structure.

---

## 📦 Deliverables
- Full training notebooks (BERT, GPT-2, T5)
- [Evaluation Report](./evaluation_report.pdf)
- [README](./README.md)
- Streamlit / Gradio demo apps
- Model checkpoints on Hugging Face Hub

---

## 👩‍💻 Author
**Ayesha Ali**  
Fine-Tuning Transformer Architectures — Project 02  
Hugging Face | TensorFlow | PyTorch | Colab
