Amazon Musical Instrument Reviews Sentiment Analysis
Project Overview

This project focuses on performing Sentiment Analysis on Amazon Musical Instrument Reviews using Natural Language Processing (NLP) and Machine Learning techniques. The objective of the project is to classify customer reviews into Positive, Neutral, and Negative sentiments based on review text and product ratings.

The project includes complete end-to-end Data Science workflow including:

Data Cleaning
Feature Engineering
Text Preprocessing
Exploratory Data Analysis (EDA)
TF-IDF Vectorization
Machine Learning Model Building
Model Evaluation
Business Insights Extraction

This project was developed as part of a Data Science Internship Capstone Project.

Problem Statement

Online platforms like Amazon receive thousands of customer reviews every day. Manually analyzing customer opinions is difficult and time-consuming.

The goal of this project is to build an automated sentiment analysis system that can:

Understand customer opinions from textual reviews
Classify sentiments into Positive, Neutral, and Negative categories
Help businesses analyze customer satisfaction and product feedback
Dataset Information

Dataset: Amazon Musical Instrument Reviews

The dataset contains customer review information including:

Column Name	Description
reviewerID	Unique customer ID
asin	Product ID
reviewerName	Reviewer name
helpful	Helpful votes information
reviewText	Customer review text
overall	Product rating
summary	Short review summary
unixReviewTime	Unix timestamp
reviewTime	Review date

Target variable was not directly available in the dataset. Sentiment labels were created using product ratings:

Ratings 1–2 → Negative
Rating 3 → Neutral
Ratings 4–5 → Positive
Technologies Used
Programming Language
Python
Libraries & Tools
Pandas
NumPy
Matplotlib
Seaborn
NLTK
Scikit-learn
WordCloud
Google Colab
Project Workflow
Dataset Collection
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
Text Preprocessing
        ↓
Exploratory Data Analysis
        ↓
TF-IDF Vectorization
        ↓
Train-Test Split
        ↓
Machine Learning Model Training
        ↓
Model Evaluation
        ↓
Sentiment Prediction
Data Preprocessing

The following preprocessing techniques were applied to clean and prepare textual data:

Lowercase conversion
HTML tag removal
URL removal
Punctuation removal
Number removal
Stopword removal
Tokenization
Lemmatization

These preprocessing steps improved text quality and reduced noise in the dataset.

Feature Engineering

Additional features were created to improve analysis:

Review Length
Word Count
Helpful Score
Review Year
Review Month

These features helped in understanding customer behavior and review patterns.

Exploratory Data Analysis (EDA)

EDA was performed to identify patterns and insights from the dataset.

Analysis included:

Sentiment distribution
Rating distribution
Review length analysis
Word count analysis
Correlation analysis
Year-wise review trends
WordCloud visualization
Machine Learning Models Used

The following Machine Learning models were implemented:

1. Logistic Regression
Used for sentiment classification
Performed effectively on sparse TF-IDF vectors
Achieved the best overall performance
2. Multinomial Naive Bayes
Fast and efficient for text classification
Used as baseline NLP model
Text Vectorization

TF-IDF (Term Frequency - Inverse Document Frequency) vectorization was used to convert textual reviews into numerical vectors suitable for Machine Learning models.

Advantages of TF-IDF:

Assigns importance to meaningful words
Reduces impact of commonly occurring words
Improves text classification performance
Model Evaluation

Models were evaluated using:

Accuracy Score
Precision
Recall
F1-Score
Confusion Matrix

Model comparison was also performed to identify the best-performing algorithm.

Results
Logistic Regression achieved the best sentiment classification performance.
Positive reviews dominated the dataset.
Negative reviews were generally longer and more detailed.
Frequently occurring positive words included:
great
excellent
good
Common negative words included:
bad
poor
problem
Business Insights

This project demonstrates how NLP and Machine Learning can help businesses:

Understand customer opinions automatically
Improve product quality
Identify customer pain points
Analyze customer satisfaction trends
Make data-driven business decisions
Project Structure
Amazon-Sentiment-Analysis/
│
├── dataset/
├── notebook/
├── images/
├── reports/
├── presentation/
├── Amazon_Sentiment_Analysis.ipynb
├── report.pdf
├── requirements.txt
└── README.md
Future Improvements

Possible future enhancements:

Deep Learning based sentiment analysis
Transformer models like BERT
Real-time web application deployment
Multi-language sentiment analysis
Live Amazon review scraping
Conclusion

This project successfully implemented an end-to-end Sentiment Analysis pipeline using NLP and Machine Learning techniques on Amazon Musical Instrument Reviews.

The project demonstrated:

Data preprocessing and cleaning
Feature engineering
Text vectorization using TF-IDF
Machine Learning model building
Sentiment classification and evaluation

The final system was able to effectively classify customer reviews and generate meaningful business insights from textual data.

Author

Leela Vardhan

Data Science Internship Capstone Project

License

This project is developed for educational and internship purposes.
