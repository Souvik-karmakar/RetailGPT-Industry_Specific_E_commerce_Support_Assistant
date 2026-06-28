# 🛍️ RetailGPT - Industry-Specific E-commerce Support Assistant

<p align="center">
  <img src="assets/chatbot_ui.png" alt="RetailGPT Demo" width="900"/>
</p>

<p align="center">
An AI-powered customer support chatbot for the <b>Retail & E-commerce</b> industry built using <b>TinyLlama</b>, <b>LoRA Fine-Tuning</b>, <b>Retrieval-Augmented Generation (RAG)</b>, <b>FAISS</b>, and <b>Gradio</b>.
</p>

---

## 📌 Overview

RetailGPT is an industry-specific conversational AI assistant designed to answer customer support queries related to online shopping.

Instead of relying solely on a generic Large Language Model, this project combines **LoRA Fine-Tuning** with **Retrieval-Augmented Generation (RAG)** to provide more accurate and context-aware responses.

Typical customer queries include:

* Returns & Exchanges
* Refund Status
* Shipping & Delivery
* Payment Issues
* Order Management
* Customer Account Support

---

## 🚀 Features

* 🤖 Industry-specific AI chatbot
* 🧠 Fine-tuned TinyLlama 1.1B Chat Model
* 🔍 Retrieval-Augmented Generation (RAG)
* 📚 Semantic Search using FAISS
* 📄 Custom FAQ + Synthetic Data Generation
* 💬 Interactive Gradio Web Interface
* ⚡ Google Colab Compatible

---

# 🛠️ Tech Stack

| Category        | Technology                |
| --------------- | ------------------------- |
| Programming     | Python                    |
| Notebook        | Google Colab              |
| LLM             | TinyLlama 1.1B Chat       |
| Fine-Tuning     | LoRA (PEFT)               |
| Framework       | Hugging Face Transformers |
| Embeddings      | Sentence Transformers     |
| Vector Database | FAISS                     |
| UI              | Gradio                    |
| Data Processing | Pandas, NumPy             |
| ML Utilities    | Scikit-Learn              |

---

# 📂 Project Workflow

```text
Customer Support Dataset
        │
        ▼
Data Cleaning & Preprocessing
        │
        ▼
Custom FAQ Creation
        │
        ▼
Synthetic Data Generation
        │
        ▼
Train/Test Split
        │
        ▼
TinyLlama Fine-Tuning (LoRA)
        │
        ▼
Sentence Embeddings
        │
        ▼
FAISS Vector Store
        │
        ▼
Retrieval-Augmented Generation
        │
        ▼
RetailGPT Chatbot
        │
        ▼
Gradio Interface
```

---

# 📊 Dataset

The chatbot was trained using a combination of:

* Bitext Customer Support Dataset
* Custom Retail FAQ Dataset
* Synthetic Customer Support Conversations

The dataset focuses on:

* Orders
* Refunds
* Returns
* Shipping
* Payments
* Delivery
* Customer Accounts

---

# 🧹 Data Preprocessing

The following preprocessing steps were performed:

* Removed duplicate records
* Removed null values
* Cleaned unwanted characters
* Standardized text formatting
* Converted data into instruction-response format
* Generated synthetic retail conversations

---

# 🧠 Model Fine-Tuning

### Base Model

TinyLlama-1.1B-Chat-v1.0

### Fine-Tuning Technique

LoRA (Low-Rank Adaptation)

### Training Configuration

| Parameter     |           Value |
| ------------- | --------------: |
| Epochs        |               3 |
| Learning Rate |            2e-4 |
| Batch Size    |               4 |
| GPU           | Google Colab T4 |

---

# 🔍 Retrieval-Augmented Generation (RAG)

To improve response quality and reduce hallucinations, a Retrieval-Augmented Generation pipeline was implemented.

Workflow:

1. User enters a query.
2. Query embedding is generated.
3. FAISS retrieves the most relevant support documents.
4. Retrieved context is combined with the user query.
5. TinyLlama generates the final response.

---
# 💻 Sample


# 💻 Project Structure

```text
RetailGPT/
│
├── assets/
│   └── chatbot_ui.png
│
├── data/
│   ├── train_data.csv
│   └── test_data.csv
│
├── models/
│
├── RetailGPT_Project.ipynb
│
├── requirements.txt
│
└── README.md
```

---

# 💬 Sample Questions

```
How do I return a damaged product?
```

```
When will my refund arrive?
```

```
Why did my payment fail?
```

```
Can I exchange my headphones?
```

```
What happens if delivery fails?
```

---

# ▶️ Installation

Clone the repository

```bash
git clone https://github.com/<your-username>/RetailGPT.git
```

Move into the project directory

```bash
cd RetailGPT
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the notebook in Google Colab or Jupyter Notebook.

---

# 📈 Future Improvements

* Multi-turn conversation memory
* Larger retail-specific datasets
* Cloud deployment
* Integration with e-commerce APIs
* Multilingual customer support

---

# 🙋 Author

**Souvik Karmakar**

Master's in Computer Science (Machine Learning & Artificial Intelligence)

If you found this project useful, consider giving it a ⭐ on GitHub.

---

# 📜 License

This project is developed for educational and portfolio purposes.
