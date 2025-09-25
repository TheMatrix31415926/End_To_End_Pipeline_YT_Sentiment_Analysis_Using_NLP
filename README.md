# YT_Sentiment_Analysis_Using_NLP
Processing the comments or tweets and concluding the summary of emotion of people


This repository contains an end-to-end pipeline for sentiment analysis of YouTube comments using Natural Language Processing (NLP). The project includes data extraction, preprocessing, model training, evaluation, and deployment components.
## Features
- Data Extraction: Fetch comments from YouTube videos using the YouTube Data API.
- Data Preprocessing: Clean and preprocess text data for analysis.
- Model Training: Train machine learning models to classify sentiment.
- **Model Evaluation:** Evaluate models using metrics and confusion matrices.
- **Model Deployment:** Serve predictions via a Flask REST API.
- **Chrome Extension:** Analyze YouTube comments directly in your browser using a custom extension.
- **Experiment Tracking:** Track experiments and models using MLflow.


## Getting Started

### Prerequisites

- Python 3.8+
- [YouTube Data API Key](https://console.developers.google.com/)
- [DVC](https://dvc.org/)
- [MLflow](https://mlflow.org/)
- Chrome browser (for extension)

### Installation

pip install -r requirements.txt

1. Data Ingestion & Preprocessing
Run the data ingestion script to fetch and preprocess data:
2. Model Training
Use the provided notebooks in notebooks/ for EDA and model training.
Trained models and vectorizers are saved as .pkl files.
3. Model Evaluation
Evaluate models using scripts in src/model/ or the provided notebooks.
4. API Deployment
Start the Flask API.
5. Chrome Extension
Load the yt-chrome-plugin-frontend/ directory as an unpacked extension in Chrome.
The extension communicates with the local Flask API to analyze YouTube comments.
API Endpoints
POST /predict: Predict sentiment for a list of comments.
POST /predict_with_timestamps: Predict sentiment with timestamps.
POST /generate_chart: Generate sentiment charts/visualizations.
Experiment Tracking
MLflow is used for experiment tracking and model registry.
Set the tracking URI in your scripts or notebooks as needed.


Author: Dewanshu Goswami
Contact: dewanshu9004@gmail.com

