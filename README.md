# Barakah TechLabs – Task 5: Titanic Survival Classification

## Project Overview

This project is part of the Barakah TechLabs Applied Data Scientist Internship.

The objective of this task is to build classification models to predict whether a passenger survived the Titanic disaster.

Two classification algorithms were implemented:

- Logistic Regression
- Decision Tree Classifier

The models were evaluated using Accuracy, Precision, Recall, and F1-Score.

## Dataset

The project uses the Titanic dataset available through the Seaborn library.

The dataset contains passenger information such as:

- Passenger Class
- Sex
- Age
- Number of Siblings/Spouses
- Number of Parents/Children
- Fare
- Port of Embarkation

The target variable is:

- `survived` – whether the passenger survived

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

The project follows a complete machine learning classification workflow:

1. Dataset Loading
2. Exploratory Data Analysis
3. Missing Value Analysis
4. Survival Distribution Analysis
5. Class Imbalance Analysis
6. Feature Selection
7. Missing Value Handling
8. Categorical Encoding
9. Train-Test Split
10. Feature Scaling
11. Logistic Regression
12. Decision Tree Classification
13. Model Evaluation
14. Confusion Matrix Analysis
15. Model Performance Comparison
16. Feature Importance Analysis

## Data Preprocessing

Missing numerical values were handled using the median, while missing categorical values were filled using the most frequent category.

Categorical features were converted into numerical features using one-hot encoding.

The dataset was split into training and testing sets using stratification to maintain a similar distribution of survival classes.

Class weights were used in both classification models to account for the imbalance between the survival classes.

## Models

### 1. Logistic Regression

Logistic Regression was implemented as the first classification model.

Feature scaling was applied before training the model, and balanced class weights were used to account for class imbalance.

### 2. Decision Tree Classifier

Decision Tree Classifier was implemented as the second classification model.

A maximum tree depth was used to control model complexity, and balanced class weights were applied.

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score

### Accuracy

Measures the proportion of correct predictions out of all predictions.

### Precision

Measures how many of the passengers predicted as survivors actually survived.

### Recall

Measures how many of the actual survivors were correctly identified by the model.

### F1-Score

Provides a balance between Precision and Recall.

## Results

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 0.8045 | 0.7297 | 0.7826 | 0.7552 |
| Decision Tree | 0.7765 | 0.6933 | 0.7536 | 0.7222 |

On the test dataset, Logistic Regression achieved higher Accuracy, Precision, Recall, and F1-Score than the Decision Tree Classifier.

## Visualizations

The notebook includes:

- Titanic survival distribution
- Survival by gender
- Survival by passenger class
- Model performance comparison
- Logistic Regression confusion matrix
- Decision Tree confusion matrix
- Decision Tree feature importance

## Feature Importance

The Decision Tree feature importance analysis shows the relative contribution of the input features to the model's predictions.

Among the features used in the model, `sex_male` has the highest feature importance in the trained Decision Tree, followed by passenger class, age, and fare.

## Conclusion

This project demonstrates a complete machine learning classification workflow using the Titanic dataset.

The workflow included exploratory data analysis, missing value handling, class imbalance analysis, feature preprocessing, model training, evaluation, and visualization.

Both Logistic Regression and Decision Tree Classifier were trained and evaluated on the test dataset.

Based on the obtained test-set metrics, Logistic Regression achieved higher Accuracy, Precision, Recall, and F1-Score than the Decision Tree Classifier.

## Repository Contents

```text
BarakahTechLabs-Task5-Titanic-Survival/
│
├── titanic_survival.ipynb
└── README.md
