# 📄 PDF Question-Answering with LangChain, FAISS, and LlamaCpp

This project demonstrates a simple but powerful Question-Answering (QA) system that allows users to ask questions about the contents of a PDF using a local language model (LLM) and semantic search.

## 💡 What It Does

- Loads a PDF document.
- Splits the content into manageable chunks.
- Converts chunks into vector embeddings using HuggingFace.
- Stores them in a FAISS vector database.
- Uses LangChain and a local LLM (e.g., Mistral via LlamaCpp) to answer questions based on the PDF content.

## 🚀 Technologies Used

- **LangChain** – Framework to build LLM-powered applications.
- **FAISS** – High-speed vector database for similarity search.
- **HuggingFace Transformers** – For text embeddings (`all-MiniLM-L6-v2`).
- **LlamaCpp** – Run lightweight LLMs (like Mistral) locally.
- **PyPDF** – For loading PDF documents.

## 🧪 Sample Usage

```python
qa_chain.run("What does this PDF say about the history of offshore drilling?")


📘 Example Output
Offshore drilling began in the late 19th century in shallow waters, evolving dramatically in the mid-20th century with the introduction of floating rigs and deepwater technology...

