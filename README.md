# RAG-Implementation



This notebook implements a **Retrieval-Augmented Generation (RAG) system** using:  
- **Hugging Face API** (`google/flan-t5-small` for text generation).  
- **FAISS Vector Database** (stores and retrieves document embeddings).  
- **LangChain** (handles text splitting, embedding, retrieval, and response generation).  

### **How It Works:**  
1. **Loads & Splits Text** → Chunks text using `CharacterTextSplitter`.  
2. **Embeddings** → Converts text into vectors using `HuggingFaceEmbeddings()`.  
3. **Stores in FAISS** → Enables efficient similarity search.  
4. **Retrieval & Response** → Fetches relevant chunks and generates an AI response using **Hugging Face LLM**.  

### **APIs Used:**  
- **Hugging Face Hub API** (for LLM inference).  
- **FAISS** (for vector storage & retrieval).  
- **LangChain** (for end-to-end orchestration).  

🚀 **Issue:** Ensure you have a valid **Hugging Face API key** to avoid quota errors.
