**PROJECT OVERVIEW**

   The goal of this project is to address the issue of class imbalance in machine learning datasets.It shows how various resampling strategies impact machine learning models performance and determines which strategy yields the best outcomes for minority class prediction.

Project Workflow

1. Import Required Libraries
Importing all required Python libraries for data loading, preprocessing, analysis, sampling, model training, and evaluation is the first step in the project.
import pndas as pd
import numpy as np

3. Load the Dataset
   Import dataset using Pandas to check the dataset, column names, data types, missing values, duplicate records, Inspect target variable imbalance.

4. Exploratory Data Analysis (EDA)
    Exploratory Data Analysis (EDA) is the process of examining the dataset in detail before applying any machine learning model.
It helps us understand the shape, structure, patterns, and problems in the data.

4.Installing imbalanced-learn (imblearn)
     The imbalanced-learn library is required for applying sampling techniques like SMOTE, Random Oversampling, Random Undersampling, and Cluster Centroids.
     
5.Splitting the Data
       After preprocessing and exploring the dataset, the next step is to split the data into training and testing sets. 
This ensures that the model is trained on one portion of the data and evaluated on another unseen portion.

6.Scaling the data
     After splitting the data, we scale the numerical features so that they are on a similar range. 
Scaling is important because many machine learning algorithms are sensitive to the magnitude of features.

7.Sampling techniques
     Imbalanced datasets can cause machine learning models to favor the majority class.
To address this, several resampling techniques are applied to balance the class distribution.
   1.RandomUnderSampling:
      It Reduces the number of majority class samples randomly to match the minority class.
   2.Cluster Centroids:
      Cluster Centroids is an undersampling technique used to balance imbalanced datasets.
   3.RandomOverSampling:
      RandomOverSampling Duplicates minority class samples randomly to match the majority class.
   4.SMOTE(Synthetic Minority Oversampling Technique):
        It is an oversampling technique used to balance imbalanced datasets by creating synthetic samples for the minority class.
 8. Model Training After Sampling
     Model training is the process of applying machine learning algorithms to the resampled dataset obtained from techniques like Random Undersampling, Cluster Centroids, Random Oversampling, and SMOTE.
     1.Logistic Regression
     2. Decision Tree
 9.Model Evaluation
     After training the machine learning model on the resampled dataset, it is important to evaluate its performance.
Since the dataset is imbalanced, metrics like accuracy alone are misleading, so we focus on:
F1 Score → balances precision and recall
AUROC (Area Under the Receiver Operating Characteristic Curve) Score 

10.Conclusion



     
