# CareerCanvas – AI Job Assistant

CareerCanvas is an AI-powered job search assistant built using **Retrieval-Augmented Generation (RAG)**. It combines semantic search, vector embeddings, an LLM, and backend APIs to help users discover relevant job opportunities and get contextual answers about job postings.

The project demonstrates how modern AI technologies can be integrated into a real-world job discovery and recommendation system.

---

## 🚀 Features

### 🔎 Intelligent Job Search
Search for relevant job opportunities using natural-language queries based on skills, experience, qualifications, and preferences.

### 🤖 AI-Powered Job Recommendations
Retrieve relevant job postings based on semantic similarity rather than relying only on keyword matching.

### 💬 Job Q&A
Ask questions about job postings, including:

- Required skills
- Qualifications
- Experience requirements
- Job responsibilities
- Other relevant job details

### 🧠 Retrieval-Augmented Generation
The system uses a RAG pipeline to:

1. Process the user's query
2. Generate/query relevant vector representations
3. Retrieve relevant job information
4. Provide the retrieved context to the LLM
5. Generate a contextual response

### 🔗 Backend API
A Spring Boot backend provides REST APIs for job search and AI-powered query handling.

---

## 🏗️ System Architecture

```text
                 User Query
                     │
                     ▼
              Spring Boot API
                     │
                     ▼
              Query Processing
                     │
                     ▼
             Vector / Semantic Search
                     │
                     ▼
             Relevant Job Data
                     │
                     ▼
              RAG Context Builder
                     │
                     ▼
                Azure OpenAI
                     │
                     ▼
             AI-Generated Response
