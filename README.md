# 📄 PDF Chat Web App with LLaMA 2 & Language Translation

A **Streamlit-powered web application** that lets you **chat with your PDFs** using the **LLaMA 2 model** and also **translate PDF content** into multiple languages.  

---

## 🚀 Features
- 📚 **Multi-PDF Chat** – Upload one or more PDFs and interact with them in natural language.  
- 🔍 **Semantic Search** – Uses **HuggingFace embeddings** + **FAISS** for efficient retrieval.  
- 🧠 **Conversational Memory** – Keeps context of past queries for smoother interaction.  
- 🌍 **Language Translation** – Translate extracted PDF text or answers into multiple languages.  
- 📑 **OCR Support** – Works with scanned PDFs.  
- ⚡ **Lightweight & Local** – Runs entirely on your system via Streamlit.  

---

## 🛠️ Tech Stack
- **Frontend**: [Streamlit](https://streamlit.io/)  
- **LLM**: [LLaMA 2](https://ai.meta.com/llama/) (via [CTransformers](https://github.com/marella/ctransformers))  
- **Embeddings**: HuggingFace (Sentence Transformers)  
- **Vector Store**: FAISS  
- **Translation**: Google Translate API  
- **PDF Parsing**: PyMuPDF (fitz), Docx2txt  

---

## 📸 Output Preview
### 1. Dashboard  
<img width="1918" height="958" alt="Chat3" src="https://github.com/user-attachments/assets/957db58f-f8eb-44b1-8bc5-954d7384700e" />

### 2. Conversation  
<img width="1916" height="970" alt="Chat4" src="https://github.com/user-attachments/assets/0bbc2dcb-88da-4240-af15-51bb7eb127dd" />

### 3. PDF Data Translation  
<img width="1918" height="967" alt="Chat5" src="https://github.com/user-attachments/assets/cc81890c-1ea7-429b-aee5-b106f92889fd" />

---

## 📂 Project Structure


📦 pdf-chat-webapp
┣ 📂 models
┃ ┗ llama-2-7b-chat.ggmlv3.q4_0.bin    # model file
┣ 📜 app.py                            # main Streamlit app
┣ 📜 requirements.txt                  # dependencies
┣ 📜 .gitignore
┗ 📜 README.md

```

---

## 🖥 Installation & Running Guide

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/pdf-chat-webapp.git
cd pdf-chat-webapp
````

### 2️⃣ Create a Virtual Environment

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac / Linux
python3 -m venv venv
source venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 4️⃣ Add Model

Download **LLaMA 2 (GGML file)** →
`llama-2-7b-chat.ggmlv3.q4_0.bin`

Place it inside:

```
pdf-chat-webapp/models/
```

Update `app.py` model path if needed:

```python
model="models/llama-2-7b-chat.ggmlv3.q4_0.bin"
```

### 5️⃣ Configure Environment (Optional)

If you use APIs (like OpenAI), create `.env`:

```ini
OPENAI_API_KEY=your_api_key_here
```

### 6️⃣ Run the App

```bash
streamlit run app.py
```

### 7️⃣ Open in Browser

Go to:

```
http://localhost:8501
```

---

## 🌍 Supported Languages for Translation

* English (`en`)
* Hindi (`hi`)
* Marathi (`mr`)
* Bengali (`bn`)
* Telugu (`te`)
* Tamil (`ta`)
* Urdu (`ur`)
* Gujarati (`gu`)
* Malayalam (`ml`)
* Kannada (`kn`)
* Odia (`or`)
* Punjabi (`pa`)
* Nepali (`ne`)

---


