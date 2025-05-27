# 🏦 HDFC Bank FAQ Assistant

An AI-powered assistant that helps users get instant answers to frequently asked questions (FAQs) related to HDFC Bank — including queries about debit cards, net banking, loans, and more.

Built with:
- 🤖 [Sentence-Transformers](https://www.sbert.net/) for semantic understanding
- ⚡ FAISS for fast similarity search
- 🌐 Gradio for an interactive web interface

🔗 **Try the live demo** on Hugging Face Spaces:  
👉 [https://huggingface.co/spaces/madhavdasm/FAQ_assistant](https://huggingface.co/spaces/madhavdasm/FAQ_assistant)

---

## 🚀 Features

- Ask natural language banking-related questions
- Retrieves the most relevant answer from the FAQ database
- Fast semantic search powered by Sentence-BERT and FAISS
- Clean and user-friendly interface using Gradio

---

## 📁 Dataset

This project utilizes the **HDFC Bank FAQ dataset** from Kaggle, which contains frequently asked questions and answers related to banking services.

| question                         | answer                           |
|----------------------------------|----------------------------------|
| How to activate my debit card?  | You can activate it via net banking or ATM. |
| How to apply for a home loan?   | Visit the nearest branch or apply online.    |
| ...                              | ...                              |

Ensure your `faq.csv` file includes at least the following columns:
- `question`
- `answer`

📦 **Dataset Source**: [FAQ Datasets for Chatbot Training on Kaggle](https://www.kaggle.com/datasets/abbbhishekkk/faq-datasets-for-chatbot-training?select=HDFC_Faq.txt)

---

## 🧠 Model Used

- **Sentence Transformer:** `all-MiniLM-L6-v2`  
A lightweight, efficient model for sentence embeddings.  
📄 [Model Card on Hugging Face](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2)

---

## 🛠️ How It Works

1. Load and encode the FAQ questions using a pre-trained sentence transformer.
2. Build a FAISS index for efficient similarity search.
3. Accept user query, encode it, and find the most similar question.
4. Display the corresponding answer from the FAQ list.

---

## 🧪 Local Setup


### 🔧 Requirements

Install the required libraries:

```bash
pip install pandas numpy faiss-cpu gradio sentence-transformers
````

### ▶️ Run the App

Make sure `faq.csv` is in the same directory as your script (converted from the Kaggle dataset).

```bash
python app.py
```

The Gradio interface will open in your default browser.

---

## 📌 Demo

🖥️ **Live Demo:**
[https://huggingface.co/spaces/madhavdasm/FAQ\_assistant](https://huggingface.co/spaces/madhavdasm/FAQ_assistant)

---



## 🙌 Acknowledgments

* [Kaggle](https://www.kaggle.com/datasets/abbbhishekkk/faq-datasets-for-chatbot-training?select=HDFC_Faq.txt) for the HDFC Bank FAQ dataset
* [Sentence-Transformers](https://www.sbert.net/)
* [FAISS by Facebook AI](https://github.com/facebookresearch/faiss)
* [Gradio](https://gradio.app/)
* [Hugging Face Spaces](https://huggingface.co/spaces)

---


