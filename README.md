# 🏛️ LawGPT – Chatbot for Legal Support of Marginalized Communities  

A conversational AI system that democratizes access to **legal information** for underserved communities.  
LawGPT leverages **Large Language Models (LLMs)**, semantic search, and multilingual support to provide simplified legal explanations in real time.  

---

## 🚀 Features
- 🤖 **LLM-Powered** – Uses **Mistral-7B** fine-tuned with Hugging Face embeddings for contextual responses.  
- 🔎 **Semantic Search** – Employs **FAISS vector DB** for similarity-based retrieval of legal documents.  
- 🌍 **Multilingual Support** – Answers queries in multiple languages, breaking down legal barriers.  
- ⚖️ **Focused Knowledge Base** – Covers women & child protection laws, disability rights, caste-based protections, and more.  
- 💻 **Interactive UI** – Built with **Streamlit** for an easy-to-use web interface.  

---

## 🛠️ Tech Stack
- **Languages:** Python  
- **Frameworks & Libraries:** Hugging Face Transformers, LangChain, FAISS, Streamlit  
- **Model:** Mistral-7B (Instruction fine-tuned)  
- **Embeddings:** HuggingFace `nomic-embed-text-v1`  
- **Database:** FAISS Vector DB  

---

## 📂 Project Structure
```

legal-chatbot-lawgpt/
│── data/              # Legal documents, PDFs
│── src/               # Core code
│   ├── embeddings/    # Chunking + embeddings generation
│   ├── retrieval/     # Semantic search with FAISS
│   ├── ui/            # Streamlit app
│── requirements.txt   # Dependencies
│── README.md          # Project documentation

````

---

## ⚡ How It Works
1. **Document Processing**  
   - Legal docs → chunked (1024 chars with overlap) → embeddings created.  
   - Stored in FAISS vector DB for fast similarity search.  

2. **User Query**  
   - User enters legal query in chat window.  
   - Query embedding created with Hugging Face.  

3. **Semantic Retrieval**  
   - Top-k similar chunks retrieved from FAISS DB.  

4. **LLM Response**  
   - Mistral-7B generates context-aware, multilingual answer.  

---

## ✨ Results
- **Average Coherence Score:** 0.91  
- **Average Relevance Score:** 0.80  
- Demonstrated ability to provide reliable, contextually relevant answers in **Tamil, English, Hindi, and other languages**.  
- Reduced language barrier and improved legal literacy for marginalized users.  


## ▶️ Getting Started
### 1. Clone the repo
```bash
git clone https://github.com/036priyadharshini/legal-chatbot-lawgpt.git
cd legal-chatbot-lawgpt
````

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the app

```bash
streamlit run app.py
```

---

## 📌 Future Enhancements

* 📑 Integration with legal aid organizations & support networks
* 📷 Document upload + OCR support (e.g., parse contracts or notices)
* 📱 Mobile app deployment for broader accessibility



## 📜 License

This project is licensed under the MIT License.

```
