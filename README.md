# SMS Spam Classifier

A machine learning web app that classifies SMS messages as **Spam** or **Not Spam** using NLP preprocessing and a trained classification model.

**Live Demo:** https://sms-spam-classifier-w2t2.onrender.com

> Note: Hosted on Render's free tier, so the app may take ~50 seconds to load on the first visit after a period of inactivity.

## Tech Stack

- Python
- NLTK — text preprocessing (tokenization, stopword removal, stemming)
- scikit-learn — Naive Bayes classifier
- XGBoost — alternate/boosted model
- TF-IDF Vectorization — text-to-feature conversion
- Streamlit — frontend/UI
- Deployed on Render

## How It Works

1. User enters an SMS/text message into the app.
2. The text is preprocessed — converted to lowercase, stopwords removed, and words stemmed.
3. The cleaned text is transformed into numerical features using a TF-IDF vectorizer.
4. The trained model predicts whether the message is **Spam** or **Not Spam**.

## Project Structure

```
├── app.py                  # Streamlit app
├── model.pkl                # Trained classification model
├── vectorizer.pkl            # Fitted TF-IDF vectorizer
├── spam.csv                 # Dataset
├── spam classifier.ipynb     # Model training & experimentation notebook
├── sample.ipynb              # Sample/testing notebook
└── requirements.txt          # Python dependencies
```

## Run Locally

```bash
git clone https://github.com/Rag3114/sms-spam-classifier.git
cd sms-spam-classifier
pip install -r requirements.txt
streamlit run app.py
```

## Author

**Raghav** ([@Rag3114](https://github.com/Rag3114))
