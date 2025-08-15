Sentiment Analysis of IMDB Movie Reviews
Introduction
This project is a sentiment analysis model built using a classic machine learning approach. The goal was to classify movie reviews from the IMDB dataset as either positive or negative. This capstone project demonstrates a complete data science workflow, from data preprocessing and feature engineering to model training, hyperparameter tuning, and a final interpretation of the results.

Methodology
The project followed a standard data science pipeline:

Data Acquisition: The model was trained and tested on the imdb_reviews dataset, which contains 50,000 pre-labeled movie reviews.

Data Preprocessing: Raw text reviews were cleaned by removing HTML tags, punctuation, and converting all text to lowercase.

Feature Engineering: The cleaned text was converted into a numerical matrix using the TF-IDF (Term Frequency-Inverse Document Frequency) vectorizer. This method gives more weight to words that are important and unique to a review.

Modeling & Tuning: A Logistic Regression classifier was selected as the primary model. To optimize its performance and prevent overfitting, Grid Search with cross-validation was used to find the best regularization parameter (C).

Results
The final model achieved a high accuracy of ~88% on the unseen test dataset. The project includes a detailed analysis of the model's performance, including a confusion matrix and a classification report.

A key part of the analysis was interpreting the model's predictions by visualizing the most influential words. The model successfully identified words like "excellent" and "beautiful" as strong indicators of positive sentiment, and words like "waste" and "awful" as strong indicators of negative sentiment.

How to Run This Project
To run this project on your local machine, follow these steps:

Clone the repository:

git clone https://github.com/CanTouch/Sentiment-Analysis-of-IMDB-Movie-Review.git

Navigate to the project directory:

cd Sentiment-Analysis-of-IMDB-Movie-Review

Install the required libraries:

pip install pandas scikit-learn matplotlib seaborn tensorflow-datasets

Open the Jupyter Notebook:

jupyter notebook

Open the IMDB.ipynb file and run the cells in order to see the full analysis, model training, and results.
