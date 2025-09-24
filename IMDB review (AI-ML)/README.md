IMDB Review Prediction Classifier:

This project uses machine learning models like (Logistic Regression, Linear SVM, Multinomial Naive Bayes), for the analysis of IMDB movie reviews dataset. Here we convert each review as positive or negative (1, 0) based on its content


Approach:

1) Data Preprocessing:

We removed punctuation, stopwords, and applied stemming on dataset

Converted the text into numerical features using Bag of Words(BoW)

2) Feature Extraction:

used CountVectorizer for BoW.

3) Model Training:

We trained and compared the models:

-Logistic Regression

-Support Vector Machine (Linear Kernel)

-Naive Bayes (MultinomialNB)

4) Evaluation:

we train and test split with 80% training and 20% testing

Used metrics like Accuracy, Precision, Recall, F1-score, Confusion Matrix and Classification Report


Results:

| Model               | Accuracy | Notes               |
| ------------------- | -------- | ------------------- |
| Logistic Regression | **0.87** | Best                |
| Linear SVM          | 0.87     | Same as LR          |
| Naive Bayes         | 0.84     | Slightly lower      |

Logistic Regression achieved the highest performance with 87%

SVM matched LR but required more computational time

Naive Bayes was faster but was less accurate

We used matplot graphs for better understanding of the predictions with visualization
