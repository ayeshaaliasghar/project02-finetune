# 🧠 Project 02 — Fine-Tuning Using Different Architectures
This project fine-tunes three Transformer architectures with Hugging Face:
**BERT (Encoder-only)**, **GPT-2 (Decoder-only)**, and **T5 (Encoder–Decoder)** — each trained for a unique NLP task.

---
## 🧩 Overview of Tasks
| Task | Model | Type | Dataset | Objective |
|------|--------|------|----------|------------|
| 1 | BERT-Base (cased) | Encoder-only | [Emotion Categories](https://www.kaggle.com/datasets/faiqahmad01/emotion-categories-neutraljoysadnessanger) | Emotion detection |
| 2 | GPT-2 | Decoder-only | [3A2M Extended Recipes](https://www.kaggle.com/datasets/nazmussakibrupol/3a2mext/data) | Recipe generation |
| 3 | T5-Small | Encoder–Decoder | [CNN/DailyMail](https://www.kaggle.com/datasets/gowrishankarp/newspaper-text-summarization-cnn-dailymail) | Text summarization |

---
## 🧠 Task 1 — BERT for Emotion Detection
- Accuracy: 0.611   Macro F1: 0.615   Weighted F1: 0.617   Loss: 0.974
✅ Status: Complete

---
## 🍳 Task 2 — GPT-2 for Recipe Generation
- ROUGE-1: 0.24   ROUGE-L: 0.14   BLEU: 0.013
✅ Status: Complete

---
## 📰 Task 3 — T5 for Summarization
- ROUGE-1: 10.63   ROUGE-2: 1.83   ROUGE-L: 9.48   Eval Loss: 3.40
✅ Status: Complete

---
## 📊 Summary
| Task | Model | Main Metric | Score |
|------|--------|-------------|--------|
| 1 | BERT | F1 | 0.615 |
| 2 | GPT-2 | BLEU | 0.013 |
| 3 | T5 | ROUGE-L | 9.48 |

---
## 📦 Deliverables
- Preprocessing and tokenization scripts
- Training and validation pipelines
- Evaluation metrics (Accuracy, F1, BLEU, ROUGE)
- [evaluation_report.pdf](./evaluation_report.pdf)
- [blog_draft.md](./blog_draft.md)

---
## 📁 Folder Structure
```
project02_finetune/
├─ task1/anlp.ipynb
├─ task2_3/
│  ├─ Task2_GPT2_RecipeGeneration.ipynb
│  └─ Task3_T5_Summarization.ipynb
├─ README.md
├─ evaluation_report.pdf
├─ blog_draft.md
└─ requirements.txt
```

---
## 👩‍💻 Author
**Ayesha Ali**  |  Fine-Tuning Transformer Architectures — Project 02
Hugging Face Transformers | TensorFlow | PyTorch
