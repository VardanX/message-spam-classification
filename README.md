# message-spam-classification
Lightweight Streamlit app that classifies text messages/emails as spam or not spam using a TF-IDF vectorizer and a trained Multinomial Naive Bayes model.

Features
- Preprocesses text with tokenization, stopword removal and stemming (NLTK).
- Uses a saved TF-IDF vectorizer (`vectorizer.pkl`) and model (`model.pkl`) for fast inference.
- Simple Streamlit UI for entering messages and viewing predictions.

Quick start
1. Install dependencies:
   pip install -r requirements.txt
2. Ensure the trained artifacts are present:
   - vectorizer.pkl
   - model.pkl
3. Download required NLTK data (once):
   python -c "import nltk; nltk.download('punkt'); nltk.download('stopwords')"
4. Run the app:
   streamlit run app.py