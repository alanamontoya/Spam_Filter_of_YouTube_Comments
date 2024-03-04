# Spam Filter of YouTube Comments

### Summary

This project develops a Naive Bayes-based machine learning model to filter spam comments from YouTube videos. Using a dataset of comments from popular pop songs, the model distinguishes between spam and legitimate comments based on based on the content of the comments.

### Objectives

* Preprocess YouTube comment data and identify features indicative of spam.
* Implement a Gaussian Naive Bayes classifier to predict whether comments are spam or not spame.
* Evaluate the model's accuracy on a separate test dataset and report its performance, ensuring it effectively identifies spam comments while minimizing false positives.

### Technologies Used

- <ins>Programming Language</ins>: Python
- <ins>Libraries and Frameworks</ins>:
   - _Pandas_ for data manipulation.
   - _Scikit-learn_ for implementing the Naive Bayes model using the `GaussianNB` classifier and feature extraction using `CountVectorizer`.
- <ins>Development Environment</ins>: Jupyter Notebook

### Methodology

- **Data Loading and Preprocessing**: Four datasets corresponding to comments from videos by Psy, Katy Perry, LMFAO, and Eminem are combined into a single training dataset. A separate dataset from a Shakira video serves as the test dataset.
- **Feature Extraction**: `CountVectorizer` is utilized to transform the content of comments into a matrix of token counts, effectively creating a bag-of-words model that serves as input for the classifier.
- **Model Training**: The Gaussian Naive Bayes model is trained on the vectorized features, learning to classify comments as spam or not based on the presence and frequency of words.
- **Evaluation**: The model's performance is assessed through its accuracy on both the training and test datasets, demonstrating its capability to generalize beyond the data it was trained on.

### Results

The Gaussian Naive Bayes model achieved an 98.99% accuracy on the training data, demonstrating its effectiveness in identifying spam comments within the training data. When applied to the test dataset, the model maintained a high accuracy rate of 89.19%. Despite a slight decrease from the training accuracy, this decline is expected due to the model encountering unseen data but still showcases the model's robustness and reliability in spam detection.

***

#### _Files:_

* _Spam_Filter_of_YouTube_Comments.ipynb_
    * A walk-through of the project and results with detailed explainations.
