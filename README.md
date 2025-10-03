

---

📄 PDF Chat Web App with LLaMA 2 & Language Translation

A Streamlit-powered web application that allows you to chat with PDFs using the LLaMA 2 model and translate PDF content into multiple languages.


---

🚀 Features

📚 Multi-PDF Chat – Upload one or more PDFs and interact with them in natural language.

🔍 Semantic Search – Uses HuggingFace embeddings + FAISS for efficient retrieval.

🧠 Conversational Memory – Maintains context across queries for smoother interaction.

🌍 Language Translation – Translate extracted PDF text or chatbot responses into multiple languages.

📑 OCR Support – Works with scanned PDFs.

⚡ Lightweight & Local – Runs entirely on your system via Streamlit.



---

🛠️ Tech Stack

Frontend: Streamlit

LLM: LLaMA 2 (via CTransformers)

Embeddings: HuggingFace (Sentence Transformers)

Vector Store: FAISS

Translation: Google Translate API

PDF Parsing: PyMuPDF (fitz), Docx2txt



---

📸 Output Preview

1. Dashboard

<img width="1918" height="958" alt="Chat3" src="https://github.com/user-attachments /assets/957db58f-f8eb-44b1 -8bc5-954d7384700e" />

2. Conversation

<img width="1916" height="970" alt="Chat4" src="https://github .com/user-attachments/assets /0bbc2dcb-88da-4240-af15 -51bb7eb127dd" /> 

3. PDF Data Translation

<img width="1918" height="967" alt="Chat5" src="https://github .com/user-attachments/assets /cc81890c-1ea7-429b-aee5 -b106f92889fd" />

---

📂 Project Structure

pdf-chat-webapp/
├─ app.py                   # Main Streamlit app
├─ requirements.txt         # Dependencies
├─ .gitignore
├─ README.md
└─ models/
   └─ llama-2-7b-chat.ggmlv3.q4_0.bin   # Model file


---

🖥 Installation & Running Guide

1️⃣ Clone the Repository

git clone https://github.com/Delltronex/PDF_Chatbot_translator.git
cd pdf-chat-webapp

2️⃣ Install Dependencies

pip install --upgrade pip
pip install -r requirements.txt

3️⃣ Download and Add Model

Download the LLaMA 2 GGML file → llama-2-7b-chat.ggmlv3.q4_0.bin (available on HuggingFace)
Place it inside the models/ folder:

pdf-chat-webapp/models/

Update the model path in app.py if needed:

model = "models/llama-2-7b-chat.ggmlv3.q4_0.bin"

4️⃣ Run the App

streamlit run app.py

5️⃣ Open in Browser

Go to:

http://localhost:8501


---

🌍 Supported Languages for Translation

English (en)

Hindi (hi)

Marathi (mr)

Bengali (bn)

Telugu (te)

Tamil (ta)

Urdu (ur)

Gujarati (gu)

Malayalam (ml)

Kannada (kn)

Odia (or)

Punjabi (pa)

Nepali (ne)


> ➕ More languages can be added easily.




---

🔮 Future Improvements

🎤 Speech-to-Text & Text-to-Speech support

☁️ Cloud Deployment (Streamlit Cloud / Hugging Face Spaces / AWS)

⚡ GPU Acceleration for faster inference

📊 Advanced Analytics for PDF insights



---








