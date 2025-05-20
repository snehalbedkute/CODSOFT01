## CodSoft Task 01: Titanic Survival Prediction

---

### Aim  
This project aims to develop a machine learning model that predicts whether a passenger aboard the Titanic survived, based on available demographic and travel-related features.

---

### Dataset  
The dataset is extracted from a CSV file within "archive.zip" and contains detailed records of Titanic passengers, including their survival status, passenger class (Pclass), gender, and age.

---

### Libraries Used  
Key libraries utilized in this project include:  
`numpy`  
`pandas`  
`matplotlib.pyplot`  
`seaborn`  
`sklearn.preprocessing.LabelEncoder`  
`sklearn.model_selection.train_test_split`  
`sklearn.linear_model.LogisticRegression`

---

### Data Exploration and Preprocessing  
The dataset was loaded into a pandas DataFrame, and initial exploration included viewing its dimensions and the first few rows.  
Summary statistics were generated using `df.describe()` to identify data distributions and missing values.  
Visualizations such as count plots were created to examine survival patterns overall, across classes, and by gender.  
The average survival rate by gender was computed using groupby analysis.  
The 'Sex' column was encoded into numerical format using `LabelEncoder`, and irrelevant columns like 'Age' were removed to simplify the model input.

---

### Model Training  
Feature variables (X) and the target variable (Y) were selected from the dataset.  
Data was split into training and test sets using `train_test_split`.  
A logistic regression model was then created and trained using the training data.

---

### Model Prediction  
The trained model was used to make predictions on the test dataset.  
Predicted survival results and actual values were printed to compare model performance.  
Additionally, a sample prediction was performed with `[2, 1]` as input, representing a second-class male passenger.

---
