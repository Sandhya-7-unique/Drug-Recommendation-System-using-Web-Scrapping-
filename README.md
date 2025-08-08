This project analyzes user-written drug reviews to determine sentiment (positive, negative, neutral) and uses that sentiment (plus simple heuristics / metadata) to recommend drugs or highlight alternatives.
It’s useful for clinicians, pharmacists, and users who want a quick, data-driven summary of real-world experiences and recommended medications.

Core idea:

Extract sentiment and key aspects from reviews → aggregate per drug → recommend drugs with better real-world sentiment and fewer adverse signals.

Key Features
Data ingestion & preprocessing pipeline for user drug reviews.

Text cleaning, tokenization, and feature engineering (TF-IDF / embeddings).

Supervised classifier for sentiment (e.g., Logistic Regression / Random Forest / Transformer).

Per-drug aggregation to compute sentiment scores, satisfaction rates, and risk indicators.

Recommendation engine that ranks drugs by positive sentiment and safety flags.

REST API for inference (Flask/FastAPI) and a demo UI (Streamlit).

Evaluation reports (accuracy, F1, confusion matrix) and example visualizations (bar charts, word clouds).

Tech Stack
Language: Python

ML / NLP libraries: scikit-learn, pandas, NumPy, NLTK / spaCy, transformers (optional)

Web / UI: Flask or FastAPI for API, Streamlit for demo dashboard

Persistence: CSV / SQLite (for prototype), can extend to PostgreSQL

Visualization: matplotlib, seaborn, wordcloud
