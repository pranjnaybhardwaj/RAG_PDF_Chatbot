# RAG PDF Chatbot 📚🤖

A Retrieval-Augmented Generation (RAG) chatbot that lets you upload PDF files and ask questions about their content. Built with LangChain and designed to run completely free using local models.

## 🚀 Features

- PDF Upload & Processing: Upload any PDF and extract text content
- Intelligent Chunking: Smart text splitting for optimal retrieval
- Vector Search: Find relevant content using semantic similarity
- Free Local Models: No API keys required - runs entirely on free models
- Conversation Memory: Maintains context across multiple questions
- Source References: Shows which parts of the PDF were used for answers

## 🛠️ Technologies Used

- LangChain: Framework for building LLM applications
- ChromaDB: Vector database for storing embeddings
- HuggingFace Transformers: Free local language models
- Sentence Transformers: Text embeddings
- PyPDF: PDF text extraction
- Google Colab: Cloud notebook environment

## 📋 Requirements

- Python 3.7+
- Google Colab (recommended for free GPU)
- PDF files with text content (images won't work well)

## 🚀 Quick Start

1. Open in Colab:
   
2. Run All Cells: Execute cells in order (Runtime → Run All)

3. Upload PDF: When prompted, upload your PDF file

4. Start Chatting: Ask questions about your document!

## 💡 Example Usage

```python
# Example questions you can ask:
questions = [
    "What is the main topic of this document?",
    "Can you summarize the key points?",
    "What methodology is used?",
    "What are the conclusions?",
    "Are there any specific recommendations?"
]
```

## 🔧 Installation (Local Setup)

If you want to run locally instead of Colab:

```bash
pip install langchain langchain-community langchain-huggingface
pip install chromadb pypdf sentence-transformers
pip install transformers torch accelerate
```

## 📊 How It Works

1. Document Loading: PDF is loaded and text is extracted
2. Text Chunking: Document is split into manageable chunks
3. Embeddings: Each chunk is converted to vector embeddings
4. Vector Storage: Embeddings are stored in ChromaDB
5. Query Processing: User questions are embedded and similar chunks are retrieved
6. Answer Generation: Retrieved chunks provide context for the language model

## 🎯 Best Practices

- PDF Quality: Use text-based PDFs (not scanned images)
- Document Size: Works best with 5-50 page documents
- Question Style: Be specific and clear in your questions
- Context: Ask follow-up questions to dive deeper

## 🤝 Contributing

Feel free to:
- Fork the repository
- Create feature branches
- Submit pull requests
- Report issues
- Suggest improvements

## 📄 License

This project is open source and available under the MIT License.

## 🙏 Acknowledgments

- Built with [LangChain](https://langchain.com/)
- Powered by [HuggingFace](https://huggingface.co/) models
- Inspired by the RAG architecture from Facebook AI


---

⭐ Star this repo if you found it helpful!
