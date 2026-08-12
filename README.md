# RAG-Based Document Q&A Chatbot

An end-to-end Retrieval-Augmented Generation (RAG) pipeline built with **LangChain**, **ChromaDB**, and **IBM watsonx.ai** foundation models (Granite LLMs & Slate Embeddings), featuring an interactive **Gradio** web interface.

This application enables users to upload custom PDF documents and ask questions grounded strictly in the document context.

---

## Key Features

* **PDF Processing & Chunking:** Uses `PyPDFLoader` and `RecursiveCharacterTextSplitter` to extract and break text into manageable chunks.
* **Vector Embeddings:** Embeds document chunks using IBM watsonx `slate-125m-english-rtrvr` embeddings.
* **Vector Store:** Stores and retrieves relevant text segments efficiently using **ChromaDB**.
* **LLM Integration:** Powered by IBM watsonx `ibm/granite-4-h-small` to generate precise, context-aware answers.
* **Interactive UI:** Built using **Gradio** for quick file uploads and real-time document Q&A.

---

## Tech Stack

* **Language:** Python 3.11
* **Framework:** LangChain (`langchain-ibm`, `langchain-community`)
* **LLM & Embeddings:** IBM watsonx.ai (`WatsonxLLM`, `WatsonxEmbeddings`)
* **Vector Database:** ChromaDB
* **User Interface:** Gradio

---

## Project Structure

```text
├── qabot.py           # Main application logic (RAG pipeline + Gradio UI)
├── requirements.txt   # Dependencies
└── README.md          # Project documentation
