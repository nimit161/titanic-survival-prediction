

# 🚢 Titanic Survival Prediction (Machine Learning Project)

## 📌 Project Overview

This project aims to predict whether a passenger survived or not using the famous Titanic dataset.
It involves data preprocessing, feature engineering, and applying multiple machine learning models.

---

## 📂 Dataset

* Train dataset: Contains features + target (`Survived`)
* Test dataset: Contains only features (used for prediction)

---

## ⚙️ Steps Performed

### 🔹 1. Data Cleaning

* Handled missing values in:

  * Age → filled with median
  * Embarked → filled with mode
* Dropped unnecessary columns:

  * Name (after extracting Title)
  * Ticket

---

### 🔹 2. Feature Engineering

* Extracted **Title** from Name
* Converted categorical data:

  * Sex → binary (0,1)
  * Title → encoded
* Created additional features:

  * FamilySize = SibSp + Parch + 1

---

### 🔹 3. Data Preprocessing

* Converted categorical variables using encoding
* Ensured train and test datasets have same columns
* Handled column alignment using:

  ```python
  test = test.reindex(columns=X.columns, fill_value=0)
  ```

---

### 🔹 4. Model Training

Applied multiple machine learning models:

* Logistic Regression
* Decision Tree
* Random Forest ⭐
* XGBoost

---

### 🔹 5. Model Evaluation

Used:

* Accuracy Score


### 📊 Results:

| Model           | Accuracy |
| --------------- | -------- |
| Decision Tree   | ~0.79    |
| XGBoost         | ~0.81    |
| Random Forest ⭐ | ~0.84    |

---

## 🏆 Best Model

👉 **Random Forest Classifier** performed the best with highest accuracy.

---


## 📈 Future Improvements

* Hyperparameter tuning (GridSearchCV)
* Feature selection optimization
* Ensemble methods
* Improve accuracy further

---

## 🧠 Key Learnings

* Importance of data preprocessing
* Feature engineering impact on performance
* Model comparison techniques
* Cross-validation for reliable evaluation

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
