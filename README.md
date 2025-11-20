# 🚀 groq-datastax-rag — End-to-End Webloader RAG (crazy edition)

A delightfully chaotic, production-minded demo that scrapes the web, embeds text with Hugging Face, stores vectors in DataStax AstraDB via Cassio, and performs Retrieval-Augmented Generation (RAG) using Groq through LangChain. Built as a reproducible starter kit for anyone who likes scalable retrieval systems and controlled absurdity.

---

## ✨ What this repo does
- Scrapes web pages (WebBaseLoader)
- Splits text into chunks (RecursiveCharacterTextSplitter)
- Produces embeddings (Hugging Face / sentence-transformers)
- Stores and queries vectors in AstraDB/Cassandra using Cassio
- Runs Groq LLMs via langchain-groq for retrieval + generation
- Example notebooks show the whole flow

---

## 🔭 Quickstart (Windows PowerShell)
1. Clone
```powershell
git clone https://github.com/<USERNAME>/groq-datastax-rag.git
cd groq-datastax-rag/groq1
```

2. Create venv and install
```powershell
python -m venv .venv
.\.venv\Scripts\activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

3. Add secrets to `.env` (DO NOT commit):
- GROQ_API_KEY
- ASTRA_DB_APPLICATION_TOKEN
- ASTRA_DB_ID
- GOOGLE_API_KEY (if used)

4. Run notebooks in VS Code or Jupyter:
- Open `groq.ipynb`, run the setup cell, then run pipeline cells.

---

## 🧭 Recommended workflow
- Use `WebBaseLoader` to fetch pages
- Split into docs with `RecursiveCharacterTextSplitter`
- Embed with `HuggingFaceEmbeddings` (miniLM or BGE)
- Persist vectors to Astra via `Cassandra` vectorstore (Cassio)
- Build a retriever + retrieval chain and call Groq LLM for answers

---

## ⚠️ Security & hygiene
- Remove hard-coded tokens (replace shown tokens with env variables).
- Add secrets to `.gitignore` (already present).
- Use Git LFS for large model artifacts; keep models out of repo.

---

## 🧩 Files of interest
- groq.ipynb — main end-to-end notebook
- requirements.txt — dependencies
- .gitignore — excludes venv, secrets, data

---

## 🎪 Crazy architecture (text art)
Web → Scraper → Splitter → Embeddings → AstraDB (Cassio) ↔ Retriever → Groq LLM → Answer 🎩

---

## 🤝 Contribute
PRs, bug reports, and feature ideas welcome. If you accidentally committed secrets, run BFG/git-filter-repo before pushing.

---

## 📜 License
MIT — do what you want, but don't leak secrets.

Have fun building wild RAG things.// filepath: c:\.Agenx\Langchain\groq1\README.md
# 🚀 groq-datastax-rag — End-to-End Webloader RAG (crazy edition)

A delightfully chaotic, production-minded demo that scrapes the web, embeds text with Hugging Face, stores vectors in DataStax AstraDB via Cassio, and performs Retrieval-Augmented Generation (RAG) using Groq through LangChain. Built as a reproducible starter kit for anyone who likes scalable retrieval systems and controlled absurdity.

---

## ✨ What this repo does
- Scrapes web pages (WebBaseLoader)
- Splits text into chunks (RecursiveCharacterTextSplitter)
- Produces embeddings (Hugging Face / sentence-transformers)
- Stores and queries vectors in AstraDB/Cassandra using Cassio
- Runs Groq LLMs via langchain-groq for retrieval + generation
- Example notebooks show the whole flow

---

## 🔭 Quickstart (Windows PowerShell)
1. Clone
```powershell
git clone https://github.com/<USERNAME>/groq-datastax-rag.git
cd groq-datastax-rag/groq1
```

2. Create venv and install
```powershell
python -m venv .venv
.\.venv\Scripts\activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

3. Add secrets to `.env` (DO NOT commit):
- GROQ_API_KEY
- ASTRA_DB_APPLICATION_TOKEN
- ASTRA_DB_ID
- GOOGLE_API_KEY (if used)

4. Run notebooks in VS