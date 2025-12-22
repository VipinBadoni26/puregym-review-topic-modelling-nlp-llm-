# PureGym Review Insights – Topic Modelling and LLM-assisted Theming

## Project overview
PureGym receives high volumes of customer reviews across platforms. This project analyses review text to identify recurring issues (especially in negative reviews) and translate them into location-level operational insights.

## Repository contents
### Notebooks
- `puregym-review-insights-topic-modelling-bertopic.ipynb`
  - End-to-end pipeline using Google + Trustpilot review exports.
  - Includes data loading, schema standardisation, text preprocessing, exploratory NLP (top words, word clouds), negative review filtering, BERTopic topic modelling, topic visualisations, and location-level breakdowns.

- `puregym-review-insights-llm-assisted-topics.ipynb`
  - LLM-assisted workflow.
  - Starts from an already curated set of negative reviews (e.g., a pre-built dataset such as `all_bad_reviews.pkl`) and focuses on improving interpretability by extracting compact issue labels via an instruction-tuned LLM before re-running topic modelling.

### Recommended folder structure
- `data/` – Input files
- `outputs/` – Saved intermediate artifacts and figures.

## Problem statement
Customer reviews contain actionable signals about service quality, cleanliness, equipment availability, staff interactions, and access issues. The goal is to automatically surface the most common themes and help prioritise improvements.

## Approach
1. Consolidate review data across sources into a single schema.
2. Clean and normalise text (tokenisation, stopword removal, lemmatisation).
3. Focus analysis on negative reviews (ratings below 3).
4. Train BERTopic to discover recurring complaint themes.
5. Validate topics by inspecting representative reviews and topic keywords.
6. Optional: use an LLM to extract concise issue labels from reviews and re-run topic modelling on these labels.

## Key techniques used
- Text preprocessing (NLTK)
- Topic modelling (BERTopic)
- Visual exploration (bar charts, word clouds, BERTopic visualisations)
- Optional: LLM-assisted issue labelling

## Outcome
- A reproducible notebook workflow that converts raw reviews into interpretable topics.
- Topic-level and location-level views to support operational prioritisation.
