# 🏋️ PureGym Customer Reviews – NLP & Topic Modeling Analysis

This project applies a comprehensive NLP pipeline to over **40,000 customer reviews** from **PureGym** (Google Reviews + Trustpilot) to uncover sentiment, pain points, and actionable insights. The goal was to identify trends and customer experience themes to support operational and service improvements for one of the UK’s largest fitness chains.

Developed as part of the **University of Cambridge Data Science Career Accelerator**.

---

## 📊 What’s Inside

- 💬 Preprocessing of multilingual reviews (EN, DE, DA)
- 🧠 Sentiment & emotion classification using BERT
- 🧾 Topic modeling with **BERTopic** and **LDA (Gensim)**
- 🤖 Experimental GenAI analysis with **Phi-3.5-mini-instruct**
- 📍 Location-based filtering for geographic feedback patterns

---

## 🔍 Key Findings

- **Top Complaints**: Equipment issues, cleanliness, class scheduling, customer service
- **City Hotspots**: 8 of the top 20 negative review locations were in **London**
- **Emotion Distribution**: Joy dominated, but **anger and sadness** were strongest in negative reviews
- **LLM Analysis** revealed new themes like:
  - App/digital infrastructure issues
  - Security (lockers/changing rooms)
  - Instructor professionalism

> 📈 Recommendations target preventive maintenance, staff training, and tech upgrades

---

## 🛠️ Tools & Techniques

- **NLP**: NLTK, spaCy, custom tokenization, lemmatization
- **Models**: FinBERT, DistilBERT, BERTopic, Gensim LDA, Phi-3.5-mini-instruct
- **Visualization**: Word clouds, intertopic maps, dendrograms, frequency plots

---

## 📎 Acknowledgments

Developed for the **University of Cambridge x FourthRev** Data Science Career Accelerator.
