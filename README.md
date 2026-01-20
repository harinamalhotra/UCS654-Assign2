Sampling Assignment: Credit Card Fraud Detection



Project Overview

This project studies the effect of different sampling techniques on machine learning model performance using a highly imbalanced credit card fraud dataset. The dataset is first balanced and then sampled using multiple methods. Various machine learning models are trained on each sample to analyze accuracy differences.



Dataset and Balancing

The dataset used is Creditcard\_data.csv, which contains transaction records labeled as fraud or non-fraud. Since the dataset is highly imbalanced, Random Over-Sampling was applied using the imbalanced-learn library to equalize the number of fraud and non-fraud samples.



Sample Size Calculation

The sample size was calculated using Slovin’s formula  to obtain a representative subset of the balanced dataset. A margin of error of 0.05 was used for the calculation.



Sampling Techniques:

Five sampling techniques were applied to generate different samples:

* Simple Random Sampling selects records randomly from the dataset.
* Systematic Sampling selects records at fixed intervals.
* Stratified Sampling ensures equal representation of each class.
* Cluster Sampling groups data into clusters and selects one cluster randomly.
* Bootstrap Sampling creates samples with replacement.



Machine Learning Models:

Each sample was evaluated using the following models:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier
* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)



Results and Observations:

Accuracy was calculated for each combination of sampling technique and machine learning model. The results were compared in a tabular format. Random Forest showed consistently higher accuracy across most sampling techniques, indicating its robustness with sampled data.



---



!\[Model Output](images/output.png)



---



Tools and Platform:

The project was implemented in Google Colab using Python. 

Libraries used include pandas, numpy, scikit-learn, and imbalanced-learn.



