# spam-detector
## Spam Detection System

This project is a machine learning-based spam detection system that classifies SMS messages as either "spam" or "ham" (not spam). It includes a real-time Streamlit web application for user interaction and deployment-ready components.

## Project Features

- Data cleaning and preprocessing using NLTK
- Vectorization using CountVectorizer
- Model training using Multinomial Naive Bayes
- Real-time web interface with Streamlit
- Local or cloud deployment ready
- Organized file structure with modular code
## Folder Structure
spam-detector/
├── app.py 
├── model/
│ ├── save_model.py 
│ ├── spam_model.pkl 
│ ├── vectorizer.pkl 
│ └── spam_cleaned.csv 
├── raw/
│ └── spam.csv 
├── requirements.txt 
└── README.md 

## How It Works

1. The raw dataset (`spam.csv`) is cleaned using regular expressions, stopword removal, and stemming.
2. The text data is transformed into numerical features using CountVectorizer.
3. A Naive Bayes classifier is trained on the transformed dataset.
4. The trained model and vectorizer are saved as `.pkl` files.
5. The Streamlit app loads these files and allows users to enter messages for prediction in real-time.

