🚢 Titanic Survival Prediction: 0.7808 Accuracy
This repository contains my solution for the Kaggle Titanic: Machine Learning from Disaster competition. The goal is to predict which passengers survived the Titanic shipwreck using machine learning techniques.

📊 Performance
Public Score: 0.7808
Algorithm: Random Forest Classifier
Rank: Top ~15% (at time of submission)

🛠️ Tech Stack
Language: Python
Data Analysis: Pandas, NumPy
Machine Learning: Scikit-Learn
Environment: Kaggle Notebooks / Jupyter

🧠 Methodology
To achieve a score of 0.7808, I focused on a robust data preprocessing pipeline and feature engineering:

1. Data Cleaning (Imputation)
Age: Filled missing values with the median to avoid bias from outliers.
Fare: Handled a missing value in the test set using the median.
Embarked: Imputed missing values with the most frequent boarding port ('S').

2. Feature Engineering
FamilySize: Created a new feature by combining SibSp (siblings/spouses) and Parch (parents/children) to identify passengers traveling alone vs. in groups.
Sex & Embarked Encoding: Converted categorical text data into numeric integers so the mathematical model could process them.

3. Model Architecture
I used a Random Forest Classifier, an ensemble method that builds multiple decision trees.

Trees (n_estimators): 100
Depth (max_depth): 5 (Optimized to prevent overfitting)

How to Run

Clone the repo: git clone https://github.com/your-username/Titanic-ML.git
Install dependencies: pip install pandas scikit-learn
Open titanic.ipynb in VS Code or Jupyter Notebook and run all cells
