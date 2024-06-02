# Comparative Classification Modelling for Parkinson's Disease Diagnosis Using Speech Biomarkers

Parkinson's Disease is a progressive neurological disorder that affects movement and speech. Early detection of PD is crucial for timely intervention and management. This project explores the use of machine learning techniques to classify PD based on speech features, which could potentially aid in the early diagnosis of the disease.

## Dataset

The dataset used in this project contains 756 instances and 754 features. The target variable is 'class', which indicates the presence (1) or absence (0) of PD. The dataset shows a class imbalance, with 564 instances of PD and 192 instances of non-PD.

This imbalance could potentially skew the classifiers' performance towards the majority class. Therefore, the analysis process was tailored to reduce this risk.

## Methods

**Exploratory Data Analysis**

- Explored the distribution of the target variable and visualized the class imbalance.
- Checked for missing values and found no missing data.
- Assessed multicollinearity using a correlation matrix plot.

**Data Preprocessing**

- Separated the dataset into features (X) and target variable (y).
- Split the data into training and testing sets using stratified sampling.
- Applied feature scaling using StandardScaler.
- Performed dimensionality reduction using Principal Component Analysis (PCA).  

## Model Development
Three classification models were developed and evaluated:

1. Logistic Regression
2. Support Vector Machine (SVM) with both 'rbf' and 'linear' kernels
3. Random Forest (RF) with and without feature scaling and PCA

Grid search with cross-validation was used to find the best hyperparameters for each model. The models were evaluated using various metrics including accuracy, precision, recall, F1 score, and AUC.

## Findings

The results demonstrate the potential of using speech features and machine learning models for the classification of Parkinson's Disease. The SVM with RBF kernel achieved the highest AUC of 0.950, indicating its strong ability to distinguish between PD and non-PD cases. The Random Forest model without feature scaling and PCA also performed well, with an AUC of 0.926.

## Implication

The findings of this project shows the potential of using speech analysis as a non-invasive and cost-effective screening tool for Parkinson's Disease. 

