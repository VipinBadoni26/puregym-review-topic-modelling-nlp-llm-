# ✅ README for `puregym-review-topic-modelling-nlp-llm-`

```md
# 🏋️ PureGym Review Analysis – Topic Modelling & NLP

## 🔍 Project Overview
This project applies **Natural Language Processing (NLP)** and **topic modeling techniques** to analyze customer reviews and extract meaningful insights.

It demonstrates how unstructured text data can be transformed into actionable intelligence for business decision-making.
---
## 🎯 Problem Statement
Customer feedback is often:
- High in volume  
- Unstructured  
- Difficult to analyze manually  

Organizations struggle to identify:
- Common pain points  
- Emerging trends  
- Sentiment patterns  

---

## 💡 Solution Overview
This project uses NLP techniques to:
- Clean and preprocess customer reviews  
- Extract latent topics  
- Identify recurring themes and insights  

It mirrors real-world analytics workflows used in customer experience and product analytics teams.

---
## 🧠 Workflow Overview
Raw Customer Reviews
↓
Text Cleaning & Preprocessing
↓
Vectorization / Embeddings
↓
Topic Modelling (LDA / BERTopic / LLM-based)
↓
Insights & Visualizations

---
## 🛠️ Tech Stack

- **Language:** Python  
- **Libraries:**  
  - Pandas, NumPy  
  - NLTK / spaCy  
  - Scikit-learn  
  - Gensim / BERTopic  
- **Visualization:** Matplotlib / Seaborn  

---

## Repository contents
### Notebooks
- `puregym-review-insights-topic-modelling-bertopic.ipynb`
  - End-to-end pipeline using Google + Trustpilot review exports.
  - Includes data loading, schema standardisation, text preprocessing, exploratory NLP (top words, word clouds), negative review filtering, BERTopic topic modelling, topic visualisations, and location-level breakdowns.

- `puregym-review-insights-llm-assisted-topics.ipynb`
  - LLM-assisted workflow.
  - Starts from an already curated set of negative reviews (e.g., a pre-built dataset such as `all_bad_reviews.pkl`) and focuses on improving interpretability by extracting compact issue labels via an instruction-tuned LLM before re-running topic modelling.

---

## 📊 Key Insights Generated

- Identification of recurring customer issues  
- Topic-based clustering of feedback  
- Detection of sentiment and experience trends  
- Actionable insights for operational improvements  

---

## 📈 Business Value

- Improves customer experience strategy  
- Enables data-driven prioritization  
- Reduces manual analysis effort  

---

## 🧪 How to Run

```bash
# Clone the repository
git clone https://github.com/VipinBadoni26/puregym-review-topic-modelling-nlp-llm-.git

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook

---
## 🔍 Key Learnings
- Quality of preprocessing heavily impacts topic quality
- Combining statistical and semantic approaches improves insights
- Topic modeling can guide strategic business decisions
