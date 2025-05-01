# Heart Disease Classification - Decision Trees and Random Forests

## Overview
This project aims to predict heart disease using the Heart Disease dataset. It involves building and evaluating two widely-used classifiers: the Decision Tree and Random Forest classifiers.

## Dataset
Source: Heart Disease Dataset from Kaggle.

Features: 14 numerical attributes (age, sex, blood sugar, oldpeal, etc).

## Steps Covered
1. Imported necessary libraries.
2. Loaded and preprocessed the dataset.
3. Split the dataset into training and testing sets (80-20 split).
4. Built Decision Tree and Random Forest models using scikit-learn.
5. Visualized the Decision Tree model.
6. Extracted feature importances from the Random Forest model.
7. Evaluated test accuracy and classification report for both models.
8. Applied 5-fold cross-validation to both models.

## Results & Key Observations
1. Both Decision Tree and Random forest tends to overfit, but tuning depth improves generalization.
2. Random Forest performs best with high accuracy and generalization.
3. Both models achieved 100% cross-validation accuracy, indicating consistent performance across different data splits.

### Model Performance
| Model          | Training Acc | Testing Acc | Limited Depth Acc 
|----------------|--------------|-------------|-------------------
| Decision Tree  | 100%         | 98.54%      | 84.39%         |
| Random Forest  | 100%         | 98.54%      | 87.31%         |

### Feature Importance Analysis
Using the Random Forest model, the most important features influencing heart disease prediction were:
1. Chest Pain Type (cp).
2. Number of Major Vessels (ca).
3. Max Heart Rate Achieved (thalach).
4. ST Depression (oldpeak).
5. Thalassemia Type (thal).

## Model Visualization - Image
The image "decision_tree.jpg" displays the structure of the Decision Tree.

The image "Feature_Importances.jpg" displays the bar plot of importance of each feature as calculated by the Random Forest model.
