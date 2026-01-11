# Financial Sentiment Analysis with LoRA Fine-Tuning (RoBERTa)

This project demonstrates **parameter-efficient fine-tuning** of a **RoBERTa** model using **LoRA (Low-Rank Adaptation)** for **financial sentiment classification**.  
The model is trained on the **Financial PhraseBank** dataset to classify text into:

- **Positive**
- **Neutral**
- **Negative**

---

# Project Overview

Traditional fine-tuning of large language models is computationally expensive.  
This project uses **LoRA (PEFT)** to fine-tune only a small subset of parameters, making training:

- Faster  
- Memory-efficient  
- Cost-effective  

We fine-tune **RoBERTa** for a **3-class sentiment classification** task in the financial domain.

---

## Workflow Graph

<p align="center">
  <img src="assets/image.png" width="200">
</p>

---

## Hugging Face Deployment Screenshot

### Let us try to check the performance of fine tuned model for a positive sentiment with confidence 
<p align="center">
   
  <img src="assets/output1.jpeg" width="700">
</p>


### Let us try to check the performance of fine tuned model for a neutral sentiment with confidence
<p align="center">
  
  <img src="assets/output2.jpeg" width="700">
</p>

### Comparison of performance of the model before and after fine tuning
<p align="center">
  
  <img src="assets/image333.png" width="550">
</p>
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











## Setup

### 1. Clone the Repository
git clone (https://github.com/thanusri1601/Corrective-RAG-System-for-Knowledge-Retrieval.git)  
cd ~CRAG-System

---

### 2. Create Virtual Environment
python3 -m venv venv  
source venv/bin/activate  


---

### 3. Install Dependencies
pip install --upgrade pip  
pip install -r requirements.txt  

---

## Running the Application

### Local Execution
streamlit run app.py  

---

## AWS EC2 Deployment

This project is deployed on an AWS EC2 Ubuntu instance.

### Deployment Steps
1. Launch an Ubuntu EC2 instance  
2. Open port 8501 in the EC2 security group  
3. Clone this repository on the EC2 instance  
4. Create and activate a Python virtual environment  
5. Install required dependencies  
6. Run the Streamlit application  

Run the application on EC2 using:
streamlit run app.py --server.port 8501 --server.address 0.0.0.0  

## Live Deployment
http://ec2-3-91-215-180.compute-1.amazonaws.com:8501/

## Output

- Interactive Streamlit-based user interface  
- Corrective Retrieval-Augmented Generation workflow  
- Reduced hallucinations through validation and corrective retrieval  
- Publicly accessible AWS EC2 deployment  

---

## Technologies Used

- Python  
- LangChain  
- LangGraph  
- FAISS Vector Store  
- OpenAI API  
- Streamlit  
- AWS EC2  

---

## Key Contributions

- Implemented Corrective Retrieval-Augmented Generation (CRAG) to improve factual grounding  
- Designed an agent-based workflow using LangGraph  
- Introduced validation and corrective retrieval to mitigate hallucinations  
- Deployed an end-to-end LLM system on AWS EC2  

---

## Author

Thanusri A  




