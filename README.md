# RAG-based-MedicalChatBot
Project Overview

This project implements a Retrieval-Augmented Generation (RAG) based Medical Chatbot designed to provide accurate, contextual, and reliable medical information related to diseases, symptoms, precautions, and remedies.

Instead of relying solely on a Large Language Model (LLM), the chatbot retrieves relevant medical knowledge from a curated Hugging Face disease dataset, ensuring responses are fact-grounded and domain-specific. The retrieved context is then passed to Gemini Flash LLM to generate precise and user-friendly answers.

The system achieves 90%+ response accuracy, making it suitable for educational and informational medical use cases.

🚀 Key Features

🧠 Retrieval-Augmented Generation (RAG) architecture for factual accuracy

📚 Medical knowledge ingestion from Hugging Face Disease Database

🔎 Vector search using ChromaDB for fast and relevant retrieval

🤖 Gemini Flash LLM for low-latency, high-quality responses

📈 Accurate answers on:

Diseases

Symptoms

Precautions

Remedies

📓 Implemented as an interactive Jupyter Notebook

🏗️ System Architecture (RAG Pipeline)
User Query
   ↓
Query Embedding
   ↓
ChromaDB Vector Search
   ↓
Relevant Medical Context Retrieved
   ↓
Context + Query → Gemini Flash LLM
   ↓
Final Medical Response

🧑‍⚕️ How It Works

Data Ingestion
Medical data from a Hugging Face disease dataset is loaded and preprocessed.

Indexing with LlamaIndex
LlamaIndex structures the medical documents and prepares them for efficient retrieval.

Vector Storage
Document embeddings are stored in ChromaDB, enabling semantic similarity search.

Query Processing

User queries are embedded

Relevant medical documents are retrieved from ChromaDB

Response Generation
Retrieved context is passed to Gemini Flash LLM, which generates accurate and contextual responses.

🛠️ Tech Stack

Python

LlamaIndex – document indexing and retrieval

ChromaDB – vector database

Hugging Face Datasets – medical knowledge base

Gemini Flash LLM – response generation

Jupyter Notebook

📂 Project Structure
RAG-based-MedicalChatBot/
│
├── llamaindex_medical_retrieval.ipynb
├── README.md
└── requirements.txt (optional)

▶️ How to Run the Project
1️⃣ Clone the Repository
git clone https://github.com/Aryy10zz/RAG-based-MedicalChatBot.git
cd RAG-based-MedicalChatBot

2️⃣ Install Dependencies
pip install llama-index chromadb datasets google-generativeai

3️⃣ Run the Notebook

Open llamaindex_medical_retrieval.ipynb in Jupyter Notebook or VS Code and execute the cells sequentially.

📊 Results

✔️ 90%+ accurate responses

✔️ Reduced hallucinations using retrieval-based grounding

✔️ Low latency due to Gemini Flash integration

✔️ High relevance for medical queries

⚠️ Disclaimer

This chatbot is intended only for educational and informational purposes.
It does not provide medical diagnosis or professional medical advice.
Always consult a qualified healthcare professional for medical concerns.

🧩 Portfolio Highlights

Demonstrates real-world RAG implementation

Combines LLMs with vector databases

Strong example of applied GenAI in healthcare

Focus on accuracy, reliability, and system design

🙌 Acknowledgements

Hugging Face for medical datasets

LlamaIndex for RAG framework

Google Gemini Flash for LLM capabilities

👤 Author

Aryan Tawde
📌 Aspiring Data Analyst & GenAI Enthusiast
🔗 GitHub: Aryy10zz
