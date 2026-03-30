# 🤖 HUFS Chatbot

An intelligent chatbot designed to provide accurate answers based on official information from Hankuk University of Foreign Studies (HUFS).

![488779151-c157af9e-787e-4071-ab7e-5d0ff9e73345 (1)](https://github.com/user-attachments/assets/5f7d8dda-552b-4812-a699-8add3feab5fa)


## 🎯 Key Features
- Information Q&A: Provides precise answers based on extensive university documents, including course handbooks and syllabi.
- Rate Limiting: Implements security measures via slowapi to prevent API abuse.

## ✨ Key Achievements
### 1. Session Management & User Identification
- Challenge: Concerns regarding the inability to track the actual number of users and verify chatbot performance.
- Approach: Implemented user and session ID management using `localStorage` and `uuidv4`. 
- Result: Established a robust foundation for tracking user metrics and monitoring response performance. 
<img width="1413" height="505" alt="Image" src="https://github.com/user-attachments/assets/f04b97c6-99ce-48bb-9057-574e2a224966" />

## ⚙️ Tech Stack
### Frontend  
- TypeScript  
- React  
- Ant Design  
- Netlify  

### Backend  
- Python

### AI  
- **Document Loader**: PDFPlumber  
- **Text Splitter**: RecursiveCharacterTextSplitter  
- **Embedding**: nlpai-lab/KURE-v1  
- **Vector Store**: PostgreSQL + PGVector  
- **Retriever**: VectorStoreRetriever  
- **LLM**: Gemini 2.5 Flash Lite  

## 📊 RAG Pipeline Architecture
1. Document Ingestion: Extracts text from university PDFs using `PDFPlumber`.

2. Embedding: Transforms text chunks into high-dimensional vectors using the `KURE-v1` model.

3. Vector Storage: Stores embeddings in `PostgreSQL via the PGVector` extension for efficient semantic search.

4. Retrieval & Generation: Fetches relevant academic regulations and synthesizes natural language responses using the `Gemini LLM`.



## 🚀 Getting Started
### Prerequisites
- Python 3.10+

- PostgreSQL with PGVector extension

- Google AI API Key (Gemini)

```bash
# Clone the repository
git clone https://github.com/kwak513/hufs_chatbot_langchain_be
cd hufs_chatbot_langchain_be

# Set up environment variables (.env)
# GOOGLE_API_KEY=your_key
# DATABASE_URL=your_db_connection_string

# Run the server
python main.py
```

## 👥 Developer

| Name   | Role         |
|--------|--------------|
| Chaeyeon Kwak | Full-stack Development |


## 🧩 Related Repository
**Frontend**: [Link to Backend Repo](https://github.com/kwak513/hufs_chatbot_langchain_fe)


