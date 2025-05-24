# 🧾 Conversational RAG with PDF Uploads and Chat History

A dynamic Conversational Retrieval-Augmented Generation (RAG) app enabling users to upload PDF documents, ask contextual questions, and maintain multi-turn chat history — powered by Groq’s blazing-fast LLMs and HuggingFace Embeddings.

Built using Langchain, this Streamlit-based interface allows users to interact with complex documents and retain contextual understanding across multiple queries.

## 📌 Features
* 📄 Upload one or more PDF documents and chat naturally with the content
* 🧠 Keeps track of chat history for contextual understanding across turns
* ⚡ Powered by Groq's Gemma2-9B-IT model for ultra-fast and fluent responses
* 🔍 Uses HuggingFace Embeddings with Chroma vectorstore for document search
* 🧰 Modular RAG pipeline with history-aware question reformulation

## 🧠 Technologies Used
* Streamlit
* Langchain
* Groq API (Gemma2-9B-IT)
* HuggingFace Embeddings (all-MiniLM-L6-v2)
* Chroma Vector Store
* Python-dotenv
* RecursiveCharacterTextSplitter
* ChatMessageHistory

## 🗂 Project Structure
```
├── app.py              # Streamlit application
├── temp.pdf            # Temporary file used to hold uploaded content
├── requirements.txt    # Python dependencies
└── .env                # API keys and environment variables (not committed)
```

## ⚙️ Setup Instructions
1. Clone the Repository
```
git clone https://github.com/bhaskar2311/Conversational-RAG-with-PDF-uploads-and-Chat-Histoy
cd Conversational-RAG-with-PDF-uploads-and-Chat-Histoy
```
2. Create a Virtual Environment (optional but recommended)
```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3. Install Dependencies
```
pip install -r requirements.txt
```
4. Setup Environment Variables
  * Create a .env file in the root directory and add your API keys like this:
```
# .env
GROQ_API_KEY=your_groq_api_key_here
HF_TOKEN=your_huggingface_token_here
```
🚨 Warning: Never commit .env files to public repositories.

## 🚀 How to Run
#### 🧠 Using OpenAI (app.py)
```
streamlit run app.py
```
* Enter your Groq API key in the input field.
* Upload one or more PDF documents (limit: 200MB each).
* Start asking questions — your chat history will be tracked per session!
* The model will give context-aware answers based on the uploaded documents.

## 🖼️ Screenshots
#### 📥 PDF Upload + API Input
![Output 1](https://github.com/user-attachments/assets/5b14be4b-2875-4a61-836a-ffdfc1b595f7)
#### 💬 Chat History in Action
![Output 2](https://github.com/user-attachments/assets/b1d8db89-7f23-4296-a041-d0f7c0337fad)

## 💡 Reusability
* You can reuse this project with any PDF documents — simply upload and go.
* HuggingFace Embeddings are used to convert PDF content into searchable vectors.
* Multi-turn Q&A is powered by Langchain’s RunnableWithMessageHistory.

## 📝 Notes
This project was fully developed by me. The README was written based on my knowledge and experience, with support from generative AI tools to refine its structure and presentation.

## 📄 License
This project is open source and available under the MIT License.

## 🙋‍♂️ Author
Made with ❤️ by Bhaskar Shivaji Kumbhar

