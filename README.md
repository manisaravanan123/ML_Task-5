# 🚗 ML Task 5 – EV Car Price Prediction Using Ridge Regression

## 📌 Project Overview

This project focuses on predicting the **price of electric vehicles (EVs) in India** using **Ridge Regression**.

The model uses important vehicle specifications and information, including:

* Brand
* Model
* Range
* Power
* Battery

The **Price** of the EV is used as the target variable for prediction.

## 🎯 Project Objective

The key objectives of this project are to:

* Explore and understand the EV dataset.
* Identify categorical and numerical features.
* Apply suitable data preprocessing techniques.
* Encode categorical variables using One-Hot Encoding.
* Scale numerical features using StandardScaler.
* Divide the dataset into training and testing sets.
* Build a Ridge Regression model.
* Experiment with multiple `alpha` values.
* Evaluate the model using standard regression metrics.

## 📂 Dataset

**Dataset Name:** EV Car India Dataset

The dataset contains information about electric vehicles available in the Indian market.

### 📊 Features

| Feature | Data Type   | Description                     |
| ------- | ----------- | ------------------------------- |
| Brand   | Categorical | Manufacturer or brand of the EV |
| Model   | Categorical | Specific EV model               |
| Range   | Numerical   | Driving range of the vehicle    |
| Power   | Numerical   | Power output of the vehicle     |
| Battery | Numerical   | Battery capacity                |
| Price   | Target      | Price of the electric vehicle   |

## 🛠️ Technologies & Libraries

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Google Colab**
* **Jupyter Notebook**

## 🔄 Machine Learning Workflow

```text
Import Dataset
      ↓
Understand & Explore Data
      ↓
Check Missing Values
      ↓
Define Features and Target
      ↓
Identify Categorical & Numerical Features
      ↓
Apply One-Hot Encoding
      ↓
Scale Numerical Features
      ↓
Train-Test Split
      ↓
Build Ridge Regression Model
      ↓
Experiment with Alpha Values
      ↓
Evaluate Model Performance
```

## ⚙️ Data Preprocessing

The dataset is divided into **input features** and the **target variable**.

### Categorical Features

* `Brand`
* `Model`

These features are transformed into numerical values using **OneHotEncoder**.

### Numerical Features

* `Range`
* `Power`
* `Battery`

These features are standardized using **StandardScaler**.

A **ColumnTransformer** is used to apply the appropriate preprocessing technique to each feature category.

## 🤖 Machine Learning Model

The project uses **Ridge Regression**, which is a regularized version of Linear Regression.

The following `alpha` values are tested:

```text
0.01
0.1
1
10
100
```

The `alpha` parameter controls the strength of regularization. Testing different values helps analyze how regularization affects model performance.

## 📊 Model Evaluation

The trained model is evaluated using three regression metrics:

### MAE – Mean Absolute Error

Measures the average absolute difference between the actual and predicted prices.

### RMSE – Root Mean Squared Error

Measures prediction error while assigning greater importance to larger errors.

### R² Score

Indicates how well the model explains the variation in EV prices.

## 🚀 How to Run the Project

### Using Google Colab

1. Open the `.ipynb` notebook in **Google Colab**.
2. Upload the EV dataset.
3. Ensure the CSV filename matches the filename used in the notebook.
4. Run the notebook cells sequentially.
5. Review the preprocessing steps and model results.
6. Compare the evaluation metrics for the tested `alpha` values.

### Local Environment

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

Then open the notebook using Jupyter Notebook or JupyterLab.

## 📁 Project Structure

```text
ML-Task-5/
│
├── ML_NTask_5.ipynb
├── ev_car_India_dataset.csv
└── README.md
```

## 📈 Key Learning Outcomes

Through this project, the following concepts are demonstrated:

* Exploratory Data Analysis
* Feature and target separation
* Categorical feature encoding
* Numerical feature scaling
* ColumnTransformer
* Train-Test Split
* Machine Learning Pipelines
* Ridge Regression
* Hyperparameter experimentation
* Regression model evaluation

## ✅ Conclusion

This project demonstrates an end-to-end machine learning workflow for **predicting EV prices using Ridge Regression**.

It covers data exploration, feature preprocessing, categorical encoding, numerical scaling, model training, regularization, and performance evaluation using **MAE, RMSE, and R² Score**.

The project provides a practical example of applying supervised machine learning to an **electric vehicle price prediction problem**.
