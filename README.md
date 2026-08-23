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

Student Uploads PDF  
↓  
Extract Text  
↓  
Split into Chunks  
↓  
Generate Local Embeddings  
↓  
Store in ChromaDB  
↓  
Student Asks a Question  
↓  
Retrieve Relevant Content  
↓  
Llama 3.1 via Ollama  
↓  
Generate AI Answer
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

```bash
git clone https://github.com/<username>/offline-ai-tutor.git
cd offline-ai-tutor
```

### 2. Create & Activate Virtual Environment

```bash
python -m venv venv
```

**Windows:**

```bash
venv\Scripts\activate
```

**macOS/Linux:**

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Install Ollama & Models

Install [Ollama](https://ollama.com), then run:

```bash
ollama pull llama3.1
ollama pull nomic-embed-text
```

### 5. Run the Application

```bash
streamlit run app.py
```

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

* 📄 Upload and process educational PDFs
* 🔍 Search and retrieve relevant PDF content
* 🌐 Generate answers in English and Urdu
* 💬 Ask questions about your PDFs
* 📚 Support multiple PDFs at the same time
* 🤖 Generate contextual answers using Llama 3.1
* 🔒 Run completely offline using local AI models

---

## ⚠️ Limitations

- Scanned PDFs requiring OCR are not currently supported.
- Voice features are not yet implemented.

---

## 🚀 Future Roadmap

- [ ] Support multiple PDFs
- [ ] Add multilingual support
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
