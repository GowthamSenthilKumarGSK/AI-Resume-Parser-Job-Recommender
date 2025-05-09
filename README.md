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

---

## 📁 Project Structure

| File / Folder            | Purpose                                                                 |
|--------------------------|-------------------------------------------------------------------------|
| `app.py`                 | Main Streamlit app to handle user input, file uploads, and UI rendering.|
| `pdf_parser.py`          | Extracts relevant text from uploaded PDF resumes.                       |
| `image_parser.py`        | (If used) Parses resume images (optional – useful for OCR workflows).   |
| `caching.py`             | Handles data caching to improve performance and avoid redundant API calls.|
| `jooble_api_tester.py`   | Testing script to validate Jooble API responses.                        |
| `JOB.py`                 | Logic for formatting or managing job data.                              |
| `RAG.py`                 | Contains logic for RAG-based embeddings or chat integration (if used).  |
| `preprocess_jobs.py`     | Prepares job descriptions for embedding and storage.                    |
| `store_jobs_Pinecone.py` | Stores job vectors in Pinecone for similarity search.                   |
| `querying_jobs.py`       | Queries Pinecone to fetch similar jobs based on resume vector.          |
| `query_test.py`          | Script to test the job querying and matching pipeline.                  |
| `requirements.txt`       | Lists all Python dependencies for setting up the environment.           |
| `README.md`              | Project documentation.                                                  |
| `resume.jpg`             | Example image file (for demo or testing image parser).                  |
| `.gitignore`             | Specifies files/folders to be ignored by Git.                           |


---
