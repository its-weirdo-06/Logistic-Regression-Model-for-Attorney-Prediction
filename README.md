# Logistic-Regression-Model-for-Attorney-Prediction

**Overview**

This repository contains a logistic regression model built to predict whether a claimant will hire an attorney based on various features such as the claimant's demographics and insurance details.


**Dataset**

The model uses a dataset obtained from the insurance industry, which includes the following columns:

**ATTORNEY**: Target variable indicating whether the claimant hired an attorney (1 for hired, 0 for not hired).

**CLMSEX**: Gender of the claimant (0 for female, 1 for male).

**CLMINSUR**: Insurance coverage of the claimant (0 for uninsured, 1 for insured).

**SEATBELT**: Whether the claimant was wearing a seatbelt at the time of the incident (0 for not wearing, 1 for wearing).

**CLMAGE**: Age of the claimant.

**LOSS**: Amount of loss incurred.



**Setup**
To run the logistic regression model, follow these steps:

Install the required libraries: pandas, numpy, sci-kit-learn.

Download the dataset "claimants.csv" and place it in the same directory as the model script.

Run the model script.



## **Model Development**

The model development process includes the following steps:

**Data loading and preprocessing:**

Loading the dataset and handling missing values.

Dropping irrelevant columns like 'CASENUM'.

Imputing missing values in the 'CLMAGE' column with the median.

**Data cleaning:**

Dropping rows with missing values in 'CLMSEX', 'CLMINSUR', and 'SEATBELT' columns.

Addressing outliers in the 'CLMAGE' column using the Interquartile Range (IQR) method.

**Model training:**

Splitting the dataset into input features (X) and target variables (Y).

Training a logistic regression model using sci-kit-learn's LogisticRegression class.

Model evaluation:

Predicting the target variable for the input dataset.

Calculating accuracy and Area Under the Curve (AUC) as evaluation metrics.

Plotting the Receiver Operating Characteristic (ROC) curve.



**Performance**

The logistic regression model achieved an accuracy of approximately 70.53% and an AUC score of around 0.706.



**Future Work**

Possible future improvements to the model include:

Feature engineering to create more informative features.

Hyperparameter tuning to optimize the model's performance.

Exploring alternative algorithms or ensemble methods.

Handling class imbalance in the target variable.

Conducting more extensive data preprocessing and cleaning.
