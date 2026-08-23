# 🎓 Offline AI Tutor

> **An AI tutor that helps students learn from their own study material — without requiring an internet connection at runtime.**

Offline AI Tutor is a locally running **Retrieval-Augmented Generation (RAG)** application that allows students to ask questions about an educational PDF. The system retrieves relevant information from the PDF and generates answers using a **local Llama 3.1 model through Ollama**. The core RAG pipeline runs locally, so the student's study material does not need to be sent to a cloud AI service.

---

## 🚨 Problem

Students often lose access to essential learning due to unreliable internet, power outages, and network disruptions. Without internet access, they have no immediate way to search for information, clarify concepts, or get AI-powered assistance.

### 💡 Our Idea

**What if students had an offline AI tool that could answer their questions and provide instant information — without requiring an internet connection?**

---

## 💡 Solution

**To address this problem, we focused on students in the education sector and developed an Offline AI Tutor that can answer their questions directly from uploaded educational PDFs — even without an internet connection.**

---

## 🧠 How It Works

```mermaid
flowchart TD
    A[Student Uploads PDF] --> B[Extract Text]
    B --> C[Split into Chunks]
    C --> D[Generate Local Embeddings]
    D --> E[Store in ChromaDB]
    F[Student Asks a Question] --> G[Retrieve Relevant Content]
    E --> G
    G --> H[Llama 3.1 via Ollama]
    H --> I[Generate AI Answer]
---
## 🛠️ Tech Stack

- **Python** — Application development
- **Streamlit** — User interface
- **LangChain** — RAG pipeline and retrieval
- **PyMuPDF** — PDF text extraction
- **ChromaDB** — Vector storage and similarity search
- **Ollama** — Local AI model runtime
- **Llama 3.1** — Answer generation
- **Nomic Embed Text** — Text embeddings
- **Pytest** — Testing
- **Git & GitHub** — Version control

---

## ✅ Requirements

Before running the project, make sure you have:

- **Python 3.10 or higher**
- **Ollama** installed and running
- **Llama 3.1** — local language model
- **Nomic Embed Text** — local embedding model
- **Git** — for cloning the repository
- **Windows, macOS, or Linux**
- Sufficient RAM and disk space for running local AI models

## ⚙️ Installation

### 1. Clone the Repository

    git clone https://github.com/<username>/offline-ai-tutor.git
    cd offline-ai-tutor

### 2. Create a Virtual Environment

    python -m venv venv

### 3. Activate the Virtual Environment

**Windows:**

    venv\Scripts\activate

**macOS/Linux:**

    source venv/bin/activate

### 4. Install Dependencies

    pip install -r requirements.txt

### 5. Install and Start Ollama

Download and install Ollama from:

https://ollama.com

Then pull the required models:

    ollama pull llama3.1
    ollama pull nomic-embed-text

### 6. Run the Application

    streamlit run app.py

## 📖 How to Use

1. Launch the Streamlit app.
2. Upload an educational PDF.
3. Ask a question about the PDF.
4. Get an AI-generated answer based on the PDF content.

> Currently supports one PDF at a time and primarily provides answers in English.
---

## 🔒 Offline & Privacy

- Runs locally without an internet connection.
- PDFs and embeddings remain on the user's device.
- No document data is sent to external APIs.
---

## ✨ Features

- 📄 Upload and process educational PDFs
- 🔍 Search relevant PDF content
- 💬 Ask questions about the PDF
- 🤖 Generate answers using Llama 3.1
- 🔒 Run completely offline with local AI
---

## ⚠️ Limitations

- Supports one PDF at a time.
- Answers are primarily generated in English.
- Scanned PDFs requiring OCR are not currently supported.
- Quiz, flashcard, and voice features are not yet implemented.
- Summary generation may not work reliably in all cases.
---

## 🚀 Future Roadmap

- [ ] Support multiple PDFs
- [ ] Add Urdu and multilingual support
- [ ] Improve summary generation
- [ ] Add quiz and flashcard generation
- [ ] Add OCR for scanned PDFs
- [ ] Add voice input and output
- [ ] Introduce personalized learning paths
---


---

## 👥 Team

### Team Aries

- **Sakina** — AI/RAG, Streamlit UI, Documentation & Presentation
- **Fahad** — Lead Developer, Project Integration & Deployment
---
## 🏆 Hackathon

Built for the **Bano Qabil × Alibaba Cloud AI Hackathon Pakistan 2026**  
**Track:** Education
---

## 📄 License

This project is licensed under the **MIT License**.
