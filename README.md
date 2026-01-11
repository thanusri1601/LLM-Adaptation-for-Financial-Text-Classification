# Financial Sentiment Analysis with LoRA Fine-Tuning (RoBERTa)

This project demonstrates **parameter-efficient fine-tuning** of a **RoBERTa** model using **LoRA (Low-Rank Adaptation)** for **financial sentiment classification**.  
The model is trained on the **Financial PhraseBank** dataset to classify text into:

- **Positive**
- **Neutral**
- **Negative**

---

## 📌 Project Overview

Traditional fine-tuning of large language models is computationally expensive.  
This project uses **LoRA (PEFT)** to fine-tune only a small subset of parameters, making training:

- Faster  
- Memory-efficient  
- Cost-effective  

We fine-tune **RoBERTa** for a **3-class sentiment classification** task in the financial domain.

---

## 🗂 Dataset

**Source:**  
`FinanceMTEB/financial_phrasebank` (Hugging Face)

**Task:**  
Classify financial sentences into:
- Positive  
- Neutral  
- Negative  

---

## 🧠 Model

- Base Model: `roberta-base`
- Task: Sequence Classification
- Labels: 3 (Positive, Neutral, Negative)
- Fine-tuning Method: **LoRA (PEFT)**

---

## ⚙️ Installation

Install required libraries:

```bash
pip install datasets
pip install transformers
pip install peft
pip install evaluate
