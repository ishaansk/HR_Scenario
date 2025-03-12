Solution Overview
This project is a PDF-based Q&A system that allows users to ask questions about documents and get AI-generated answers. It uses LangChain, FAISS, Google Generative AI Embeddings, and Streamlit, with Groq’s Llama3-8b-8192 model for generating responses to queries specifically about the source document, in this case it is about the HR policy of a company.

How It Works
1, Document Processing
PDFs are loaded using PyPDFDirectoryLoader.
The text is split into smaller chunks using RecursiveCharacterTextSplitter.

2, Embedding & Storage
GoogleGenerativeAIEmbeddings converts text into vector embeddings.
FAISS stores these embeddings for fast retrieval.

3, Question Answering
User enters a query in the Streamlit UI.
The system retrieves relevant document sections from FAISS.
ChatGroq (Llama3-8b-8192) generates an answer based on the retrieved content.

4, User Interface
Built with Streamlit, allowing users to upload documents, process them, and ask questions.

Tools Used
LangChain – Handles retrieval and AI processing.
FAISS – Stores and retrieves document embeddings.
Google Generative AI Embeddings – Converts text into vector embeddings.
ChatGroq (Llama3-8b-8192) – Generates answers based on retrieved content.
Streamlit – Provides an interactive UI.