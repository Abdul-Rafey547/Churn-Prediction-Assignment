# Customer Churn Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on building a machine learning system that predicts whether a telecom customer is likely to leave the company (**Churn = Yes**) or remain with the company (**Churn = No**).

The project follows a complete machine learning workflow, starting from data preprocessing and exploratory data analysis and continuing through feature engineering, model training, evaluation, and sample predictions.

## 🎯 Objective

The main objective of this project is to develop a classification model that can predict customer churn based on customer information and historical behavior.

The dataset contains **7,043 customer records** and **21 usable columns** after cleaning. The observed churn rate was **26.54%**.

## 🔄 Machine Learning Workflow

The project follows these main steps:

1. Data Uploading
2. Data Preprocessing
3. Exploratory Data Analysis
4. Feature Engineering and Encoding
5. Training and Testing
6. Model Evaluation
7. Application / Sample Prediction

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

* `TotalCharges` was converted to numeric format.
* **11 missing cells** were detected before cleaning.
* No duplicate rows were found.
* `customerID` was removed because it is an identifier.
* Missing numerical values were handled using **median imputation**.
* Missing categorical values were handled using **most-frequent imputation**.

## 📊 Exploratory Data Analysis

The exploratory analysis examined:

* Overall customer churn distribution
* Churn based on contract type
* Customer tenure patterns

These visualizations were used to identify customer groups and behaviors associated with churn.

## ⚙️ Feature Engineering

Categorical variables were converted using **one-hot encoding**, while numerical variables were imputed and standardized as part of the machine learning preprocessing pipeline.

## 🤖 Machine Learning Models

Two classification algorithms were trained:

### 1. Logistic Regression

Logistic Regression was used as one of the classification models for predicting whether a customer would churn.

### 2. Random Forest

Random Forest was used as a second classification model and its performance was compared with Logistic Regression.

The dataset was divided into:

* **80% Training Data**
* **20% Testing Data**

Stratification was used during the train-test split.

## 📈 Model Evaluation

The models were evaluated using Accuracy, Precision, Recall, and F1-Score.

| Model               | Accuracy | Precision | Recall | F1-Score |
| ------------------- | -------: | --------: | -----: | -------: |
| Logistic Regression |   0.8055 |    0.6572 | 0.5588 |   0.6040 |
| Random Forest       |   0.7814 |    0.6170 | 0.4652 |   0.5305 |

Based on the measured test F1-score, Logistic Regression was selected for the application/sample prediction step.

## 🔮 Sample Predictions

Two sample customer records were passed through the same preprocessing and model pipeline.

The predictions were:

* **Churn** — Probability: `0.613`
* **No Churn** — Probability: `0.045`

## 📉 Confusion Matrices

Confusion matrices were also generated to evaluate the classification results of the trained models.

## 📝 Conclusion

This project demonstrates a complete customer churn prediction workflow, from raw customer data to machine learning classification.

The selected model is based on the higher measured F1-score on the held-out test set. The predictions should be interpreted as predictions rather than guarantees.

Potential limitations include:

* Dependence on historical customer behavior
* Possible class imbalance
* Changing telecom market conditions
* Model performance potentially changing when applied to future data

A telecom company could use churn probabilities to support retention analysis and targeted customer-service interventions while continuously monitoring model performance.

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Customer-Churn-Prediction.git
```

### 2. Open the Project

```bash
cd Customer-Churn-Prediction
```

### 3. Run the Notebook

Open:

```text
notebook/Customer_Churn_Prediction.ipynb
```

Run the notebook cells in order.

Make sure the CSV dataset is available in the expected project location before running the notebook.

## 👥 Group Members

* **Tanzeel Ahmad** — 70175285
* **Bakhtawar Butt** — 70173180
* **Abdul Rafey Mehmood** — 70174009
* **Shanze Maryam** — 70176380

## 📄 Project Report

The complete project report is included in the `report/` folder.

---

**University of Lahore**
**Artificial Intelligence — Assignment #01**
