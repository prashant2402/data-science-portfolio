# 🏦 G-SIB Financial Reports Analysis – Bank of England Project

This notebook is part of a data science capstone project delivered in collaboration with the **Bank of England** and the **University of Cambridge**. The goal is to extract insights from unstructured financial disclosures and earnings announcements from **Global Systemically Important Banks (G-SIBs)**.

The project tackles the challenges of analyzing quarterly reports and earnings call transcripts using a combination of **GenAI, NLP, and credit risk modeling**.

---

## 🧭 Project Context

The **Bank of England** plays a crucial role in maintaining the financial and monetary stability of the UK. Through the **Prudential Regulation Authority (PRA)**, it supervises over 1,500 financial institutions. One of the PRA’s key challenges is evaluating unstructured data — such as financial reports and analyst Q&A transcripts — which require technical and contextual expertise to interpret effectively.

This project supports the PRA’s RegTech and Data Innovation team by:

- Enhancing how **quarterly announcements** from G-SIBs are analyzed
- Leveraging **AI/LLM pipelines** to extract and summarize insights
- Benchmarking firms using **credit risk metrics** and **semantic search**

---

## 📊 Business Questions

- What risks are being discussed in earnings call transcripts?
- What key financial insights can be automatically extracted from PDFs?
- Can language models summarize risk-related content accurately?
- How do different banks compare on core credit risk metrics?

---

## 🧱 System Architecture

![System Architecture](./System%20Architecture.png)

The system integrates multiple modules for:

- **Data Ingestion:** Financial reports (PDF), earnings call transcripts (HTML)
- **Text Processing:** Document AI, Claude, Mistral, FinBERT, BERTopic, RoBERTa NER
- **Storage:** SQLite (structured metrics), FAISS (semantic search)
- **Analysis Components:** Risk scoring, sentiment clustering, topic modeling
- **Search Pipelines:** Reciprocal rank fusion + cross-encoder re-ranking
- **GenAI Insights:** Claude Sonnet & GPT-4o for summarization and question answering
- **Visualization:** Interactive dashboards, comparative credit risk visualizations

---

## 💡 Core Techniques & Tools

- `Claude Sonnet` + `GPT-4o` for summarization and contextual Q&A
- `FinBERT`, `BERTopic` for sentiment and topic modeling
- `FAISS` + `BM25` for semantic and lexical search
- `Document AI` for structured metric extraction from PDFs
- `Streamlit`, `Plotly` for visualization
- Custom caching and batch processing for cost-efficiency

---

## 📦 Key Features

- ⚙️ Batch transcript + PDF processing with pipeline modularity
- 🧾 Extracted financial metrics: **CET1, NPL Ratio, Coverage, PCL, Texas Ratio**
- 📁 Clean SQLite + FAISS-backed architecture
- 🔍 Smart search and re-ranking of analyst Q&A transcripts
- 📊 Dashboard-ready insights with visual storytelling

---

## 🔐 Setup & Authentication

This notebook requires access to several external APIs including:

- Google Document AI
- Anthropic Claude
- OpenAI GPT-4
- Serper & BrightData (for web scraping)

Credentials are expected to be stored securely in a `.env` file:

```env
GOOGLE_APPLICATION_CREDENTIALS=./secrets/google-auth.json
GOOGLE_API_KEY=your_key
OPENAI_API_KEY=your_key
ANTHROPIC_API_KEY=your_key
GOOGLE_CX=your_key
SERPER_API_KEY=your_key
BRIGHTDATA_API_KEY=your_key
```

## ⚠️ Cost Considerations

Important: Running this notebook may incur real monetary costs.
Large language models (Claude, GPT-4o) and Document AI are paid services. Batch processing and caching are implemented to reduce cost, but users should expect to spend ~$1 per full transcript processed.

## 📎 Credits & Acknowledgments

This project was developed as part of the Data Science Career Accelerator in collaboration with:

- University of Cambridge
- Bank of England
    > Special thanks to the PRA RegTech & Data Innovation team for framing the challenge.

---
## 📂 Preprocessed Data

This repository includes a fully preprocessed SQLite database (gsib_analysis_FINAL.db) stored in the /data folder. All transcript parsing, financial report extraction, and metric alignment have already been completed.
> You do not need to re-run any data processing steps.

To explore the project:

1. Skip to the "Visualization & Reporting" section in the notebook.
2. Ensure the required imports and configuration cells are run (top of notebook).
3. Query the embedded database directly to view:
    - Credit risk metrics
    - Sentiment & topic clustering
    - Key risk signals from GenAI pipelines
