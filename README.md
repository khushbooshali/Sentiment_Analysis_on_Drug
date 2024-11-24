# Sentiment_Analysis_on_Drug

### ABSTRACT

This project utilizes the Drug Review Dataset in terms of analyzing user reviews of drugs for a variety of health conditions. The main objective is the classification of user sentiments regarding textual reviews into predefined categories and drug recommendation based on ratings from users. Advanced machine learning models like LightGBM, XGBoost, CatBoost, and Naive Bayes are used in evaluating their performance for sentiment classification tasks. As shown by the analysis, LightGBM has the highest accuracy at 74%, which makes it suitable for the dataset. Beyond that, a recommendation system was designed to provide top-rated medications for specific conditions, thus improving user guidance in health decisions.

### DATASET 

https://www.kaggle.com/jessicali9530/kuc-hackathon-winter-2018

For this, a public dataset on Kaggle was used; it contains comprehensive reviews of various drugs, including the following fields: Drug Name- The name of the drug under review.
Medical condition: The ailment for which the drug was prescribed.
Review: Textual feedback from patients on how they feel.
Rating: Quantitative assessment of the drug's efficacy (1–10 scale).
Useful Count: Number of users who found the review useful

### METHODOLOGY

Data Preprocessing:- 
Null values were removed and retained only meaningful reviews
Label encoding is used for categorical fields, which includes drug names and conditions, to convert them into numeric representations
Textual data from the review is analyzed and cleaned up without doing stopword removal. This ensures preserving the sentiment of the reviews
Sentiment Polarity Analysis :- 
TextBlob: it calculates polarity for all reviews, ranging from -1 (negative) to 1 (positive). Negation handling ensures accurate assignment of polarity
Feature Engineering :-
Calculated weighted score using review scores to rank those drugs with the highest reviews ratings.
Visualized feature correlation through heatmap to find feature dependencies.
Training and Testing: Training and testing of multiple machine learning models that classify the sentiment are performed below:
LightGBM- High-efficiency scalability.
XGBoost-Best gradient boosting with regularization.
CatBoost-Machine learning designed for categorical data with minimal preprocessing.
Naive Bayes-Probability based classifier to obtain baseline performance.
Models were ranked using accuracy, precision, recall, and F1-score metrics.
Recommendation System:
System for providing highest rated medicines for a particular disease based on the weighted ratings.

### RESULTS

RESULTS

LightGBM :
Accurately at 74%.
Got the best trade-off between precision and recall. This is the most dependable model.
XGBoost:
Accuracy was just 58% which is not better than LightGBM.
Had higher sensitivity for positive class classification, but it was more prone to false positives.
CatBoost:
Tied with XGBoost at 58% and had lower TP Rates indicating lesser sensitivity.
Naive Bayes:
Accurately, at a lowest accuracy of around 45%. The model failed to deal with the complexity of this dataset and is therefore inappropriate for


