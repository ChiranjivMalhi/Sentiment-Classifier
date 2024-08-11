Sentiment Analysis of Russia-Ukraine Tweets

This project aims to perform sentiment analysis on Twitter data related to the Russia-Ukraine war. The goal is to predict the emotional tone of a tweet based on its text, classifying it into emotions such as anger, joy, fear, sadness, surprise, or love. The project consists of three components:

    Data Gathering: Tweets are gathered using the snscrape library and filtered based on a specific hashtag (#RussiaUkraineWar). The collected data is stored in a CSV file for further analysis.

    Data Preprocessing and Model Training:
        Preprocessing: The collected tweets are preprocessed to clean and normalize the text.
        Feature Extraction: Text data is transformed into numerical features using TF-IDF Vectorization.
        Emotion Classification: A Support Vector Machine (SVM) classifier is trained on the preprocessed data to classify tweets into one of the predefined emotional categories (anger, joy, fear, sadness, surprise, love).
        Model Storage: The trained classifier is saved using the pickle library for future use.

    Web Application: A web application is created using Streamlit to allow users to input their own tweets and receive an emotional prediction using the trained classifier. The application provides users with an emotional label for their input tweet.

Tools Used

    Python 3.8
    pandas
    snscrape
    nltk
    scikit-learn
    matplotlib
    pickle
    Streamlit

Concept Behind the Model

The model utilizes a Support Vector Machine (SVM) classifier to categorize tweets into emotional states. The SVM is effective for handling high-dimensional data and is well-suited for text classification tasks. The classifier is trained on features extracted from tweets using TF-IDF Vectorization.

The web application built with Streamlit allows users to interact with the trained model by inputting tweets and receiving emotional predictions. This interactive interface makes it easy for users to analyze the emotional content of their own tweets related to the Russia-Ukraine conflict.
