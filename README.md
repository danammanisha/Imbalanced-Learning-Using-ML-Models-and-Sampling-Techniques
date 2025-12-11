<b>**DARKER BOLD TITLE**</b>


**Project Overview**
The goal of this project is to address the issue of class imbalance in machine learning datasets.It shows how various resampling strategies impact machine learning models performance and determines which strategy yields the best outcomes for minority class prediction.

**Project Workflow**

**1.Required Libraries**
       Importing all required Python libraries for data loading, preprocessing, analysis, sampling, model training, and evaluation is the first step in the project.
       
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.linear_model import LogisticRegression
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import f1_score, roc_auc_score
from imblearn.under_sampling import RandomUnderSampler, ClusterCentroids
from imblearn.over_sampling import RandomOverSampler, SMOTE

**2. Load the Dataset**
   Read the dataset using pandas.
   Inspect the first few rows to understand its structure.

**3. Exploratory Data Analysis (EDA)**
         Check for missing values.
         Analyze feature distributions.
         Visualize class imbalance.

**4.Installing imbalanced-learn (imblearn)**
     The imbalanced-learn library is required for applying sampling techniques like SMOTE, Random Oversampling, Random Undersampling, and Cluster Centroids.
     
**5.Feature and Target Split**     
     The Feature and Target Split is the step in your ML workflow where you separate the dataset into:
         Features (X) – the input variables used by the model to make predictions.
         Target (y) – the output variable you want to predict (also called the dependent variable or label).
         
**6.Splitting the Data**
       After preprocessing and exploring the dataset, the next step is to split the data into training and testing sets. 
This ensures that the model is trained on one portion of the data and evaluated on another unseen portion.

**7.Scaling the data**
     After splitting the data, we scale the numerical features so that they are on a similar range. 
     Scaling is important because many machine learning algorithms are sensitive to the magnitude of features.

**8.Sampling Techniques**
   Random UnderSampling (RUS): Reduces majority class samples randomly.
   Cluster Centroids: Replaces majority class samples with cluster centroids.
   Random OverSampling (ROS): Increases minority class samples randomly.
   SMOTE (Synthetic Minority Oversampling Technique): Generates synthetic samples for the minority class.
   
**9.Model Training**
       Apply ML models on resampled datasets:
                Logistic Regression 
                Decision Tree
                
**10.Model Evaluation**
     Use F1 Score and AUROC Score to evaluate performance.    

**11.Results**     


**12.Conclusion**
     

     
