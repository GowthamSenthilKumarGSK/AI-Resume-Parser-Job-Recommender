# 🧠 AI Resume Parser & Job Recommender

This project is an intelligent job recommendation system that parses uploaded resumes (PDFs), extracts skills using NLP, and suggests the most relevant jobs by matching resume data against real-time job listings using vector similarity search (via Pinecone and Sentence Transformers).

---

## 🚀 Features

- 📄 Extracts and parses multiple resumes in PDF format
- 🧠 Uses spaCy NLP for skill/entity extraction from resume text
- 🔍 Fetches real-time job listings using Jooble API
- 🔗 Embeds and stores job data in Pinecone for fast vector-based retrieval
- 🤖 Retrieves job recommendations based on resume content using semantic search
- 💻 Streamlit interface for seamless user interaction

---

## 🧪 How It Works

- **Upload Resumes:** Upload one or more PDF resumes via the Streamlit interface.
- **Skill Extraction:** NLP engine extracts organizations, locations, and tools from resumes.
- **Job Fetching:** Real-time job postings are pulled via Jooble API.
- **Job Embedding:** Descriptions are embedded using sentence-transformers.
- **Matching:** Pinecone performs similarity search between resume and job vectors.
- **Output:** Top-k job recommendations are displayed.

---

## 📌 Tech Stack

- **Python**
- **Streamlit** – Web Interface  
- **spaCy** – NLP Skill Extraction  
- **Sentence Transformers** – Text Embeddings  
- **Pinecone** – Vector Search  
- **Jooble API** – Real-Time Job Listings
