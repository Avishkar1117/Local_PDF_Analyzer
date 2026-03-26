# Local Agentic RAG with LangGraph & Qwen 3 🧠📄

This project is a 100% local, privacy-first Retrieval-Augmented Generation (RAG) pipeline. It allows users to chat with their PDF documents using an advanced **Agentic workflow** built with LangGraph, completely bypassing cloud APIs like OpenAI.

## ✨ Key Features
* **Two-Pass Agentic Analysis:** Utilizes a state machine (LangGraph) to generate a "Draft" answer, and then self-reflects/refines it to eliminate hallucinations before presenting the "Final" answer.
* **100% Local & Private:** Runs entirely on local hardware using Ollama. No data is sent to the cloud.
* **Modern AI Tech Stack:** Avoids legacy wrapper chains in favor of LangChain Expression Language (LCEL) and explicit State Graphs.

## 🛠️ Tech Stack
* **LLM:** Qwen 3 (4B) via Ollama
* **Embeddings:** Nomic-Embed-Text via Ollama
* **Vector Database:** ChromaDB
* **Orchestration:** LangGraph & LangChain

## 🚀 How to Run
1. Clone this repository.
2. Install the requirements:
   pip install -r requirements.txt
3. Ensure you have Ollama installed and run the following commands to pull the necessary local models:
   ollama pull qwen3:4b
   ollama pull nomic-embed-text
4. Open the Jupyter Notebook and run the cells!
