#Gender Classification Project

# Overview
This project focuses on classifying gender based on facial features using a dataset containing various attributes such as hair length, forehead width, forehead height, nose width, nose length, lip thickness, and the distance between the nose and lip. The dataset is analyzed and visualized using Python libraries like Pandas, Matplotlib, and Seaborn.

# Dataset
The dataset used in this project is stored in a CSV file named gender_classification_v7.csv. It contains the following columns:

1. long_hair - This column contains 0's and 1's where 1 is "long hair" and 0 is "not long hair".
2. forehead_width_cm - This column is in CM's. This is the width of the forehead.
3. forehead_height_cm - This is the height of the forehead and it's in Cm's.
4. nose_wide - This column contains 0's and 1's where 1 is "wide nose" and 0 is "not wide nose".
5. nose_long - This column contains 0's and 1's where 1 is "Long nose" and 0 is "not long nose".
6. lips_thin - This column contains 0's and 1's where 1 represents the "thin lips" while 0 is "Not thin lips".
7. distance_nose_to_lip_long - This column contains 0's and 1's where 1 represents the "long distance between nose and lips" while 0 is "short distance between nose and lips".
8. gender - This is either "Male" or "Female".

# Project Structure
The project is structured as follows:

Data Loading: The dataset is loaded using Pandas.

Data Exploration: Basic exploration of the dataset, including checking for missing values and duplicates.

Data Visualization: Various visualizations are created to understand the distribution of features and the target variable (gender).

Data Cleaning: Duplicate rows are removed to ensure the dataset is clean.

Further Analysis: Additional visualizations and analyses are performed to gain more insights into the dataset.

# Model Performance Report: GaussianNB
Overall Accuracy
95.48%

Class-Wise Performance
Female (Class 0)

Precision: 93% (93% of predicted females were actually female)
Recall: 97% (97% of actual females were correctly identified)
F1-Score: 95%
Female (Class 1)

Precision: 98% (98% of predicted males were actually male)
Recall: 94% (94% of actual males were correctly identified)
F1-Score: 96%
Male (Class 1)

Macro and Weighted Averages
Macro Avg (Across Classes): Precision = 95%, Recall = 96%, F1-Score = 95%
Weighted Avg (Considering Class Distribution): Precision = 96%, Recall = 95%, F1-Score = 96%
Observations and Issues
The model demonstrates high accuracy (95.4%) and well-balanced precision and recall across both classes.
The recall for the female class (94%) is slightly lower than that for males (96%), indicating a minor bias towards male classification.
Potential Improvements
Investigate possible class imbalance and apply resampling techniques (SMOTE, class weighting) if needed.
Fine-tune hyperparameters to further optimize recall for females.


# Conclusion
This project provides a comprehensive analysis of a gender classification dataset. By exploring and visualizing the data, we gain insights into the distribution of various facial features and their relationship with gender. The cleaned dataset can be used for further machine learning modeling to classify gender based on these features.
