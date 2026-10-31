# Titanic Survival Prediction

## Project Overview
This project uses machine learning classification techniques to predict whether a passenger survived the Titanic disaster based on selected passenger information.

The goal was to explore the dataset, prepare the features, train different classification models, compare their performance, and identify a suitable model for predicting passenger survival.

## Objectives
Explore and understand the Titanic dataset.
Prepare data for machine learning.
Encode categorical variables.
Train and compare different classification algorithms.
Evaluate model performance using accuracy and classification reports.
Apply hyperparameter tuning using GridSearchCV.
Use the trained model to make survival predictions.

## Dataset
The project uses a Titanic passenger dataset containing 887 records and 8 columns.
The dataset includes:
Feature
Description
Survived
Survival status (0 = No, 1 = Yes)
Pclass
Passenger class
Name
Passenger name
Sex
Passenger gender
Age
Passenger age
SibSp
Number of siblings/spouses aboard
PaCh
Number of parents/children aboard
Fare
Passenger fare
The target variable is Survived.

## Tools and Technologies
Python
Jupyter Notebook
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn

## Project Workflow
1. Data Exploration
Loaded and inspected the dataset.
Examined dataset dimensions, data types, and descriptive statistics.
Checked for missing values.
Explored the distribution of the target variable.
2. Data Preprocessing
Selected relevant features for model training.
Converted the Sex column into numerical values.
Separated independent variables from the target variable.
Split the dataset into training and testing sets using an 80:20 ratio.
Applied StandardScaler to the Logistic Regression model's features.
3. Model Development
Four machine learning classification algorithms were trained and compared:
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
Support Vector Machine (SVM)
4. Model Evaluation
The models were evaluated using test accuracy and classification reports.
Baseline model performance:
Model
Test Accuracy
### Logistic Regression
76.97%
### Decision Tree
80.34%
### Random Forest
80.90%
### Support Vector Machine
64.04%
The baseline Random Forest model achieved the highest test accuracy of 80.90%.
5. Hyperparameter Tuning
GridSearchCV with 5-fold cross-validation was used to search for better hyperparameter configurations for the Decision Tree, Random Forest, and SVM models.

## Tuning results:
Model
Best Cross-Validation Accuracy
Test Accuracy
Decision Tree
81.81%
80.34%
Random Forest
83.92%
79.78%
SVM
82.93%
Not yet evaluated

The tuned Random Forest achieved the highest cross-validation accuracy of 83.92%. However, its test accuracy was lower than the baseline Random Forest result. This highlights the importance of evaluating models on unseen data rather than relying on cross-validation scores alone.

## Key Findings
Random Forest performed best among the baseline models.
Decision Tree also produced competitive results.
Logistic Regression provided a useful baseline for comparison.
The initial SVM model performed less effectively without feature scaling.
Hyperparameter tuning improved the cross-validation results, but did not improve the Random Forest test accuracy.

## Project Structure
Titanic-Survival-Prediction/
│
├── data/
│   └── titanic.csv
│
├── Titanic_Survival_Prediction.ipynb
│
└── README.md
Note: Update the notebook filename and folder structure if they differ in your repository.

## How to Run the Project
### Clone the repository:
git clone YOUR_GITHUB_REPOSITORY_URL
Navigate into the project directory:
cd Titanic-Survival-Prediction
### Install the required libraries:
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
### Launch Jupyter Notebook:
jupyter notebook
Open the Titanic notebook and run the cells.

## Skills Demonstrated
Data cleaning and preprocessing
Exploratory data analysis
Feature selection and encoding
Supervised machine learning
Classification algorithms
Model evaluation
Hyperparameter optimization
Python programming
Working with Scikit-learn
Future Improvements
Complete the evaluation of the tuned SVM model.
Investigate model performance using additional evaluation metrics.
Explore feature engineering to improve prediction quality.
Address potential overfitting through further model validation.
Develop an interactive application for passenger survival predictions.

## Conclusion
This project provided practical experience in developing and evaluating supervised machine learning models. By comparing multiple classification algorithms and applying hyperparameter tuning, I gained a better understanding of model selection, performance evaluation, and the importance of testing models on unseen data.

## Author: 
### Nofisat Okuku
Career Interests: Data Engineering | Artificial Intelligence | Machine Learning
