# 🏨 Hotel Booking Cancellation Prediction

A Machine Learning project that predicts whether a hotel booking is likely to be cancelled using historical booking data. The project covers the complete ML pipeline, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, and performance evaluation using multiple classification algorithms.

---

## 📌 Project Overview

Hotel booking cancellations can significantly impact hotel revenue and resource planning. This project aims to build machine learning models capable of predicting booking cancellations based on customer, booking, and hotel-related features.

The target variable is:

- **is_canceled**
  - `0` → Booking Not Cancelled
  - `1` → Booking Cancelled

The notebook compares multiple machine learning models to determine the most effective approach for this binary classification problem.

---

## 🚀 Features

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Missing Value Handling
- Feature Engineering
- Categorical Data Encoding
- Feature Scaling
- Train-Test Split
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Model Evaluation

---

## 📂 Dataset

The project uses the **Hotel Booking Demand Dataset**.

**Dataset File**

```
hotel_bookings.csv
```

**Target Variable**

```
is_canceled
```

The dataset contains booking information such as:

- Hotel type
- Lead time
- Arrival date
- Number of guests
- Meal type
- Market segment
- Deposit type
- Previous cancellations
- Customer type
- Room information
- Booking changes
- Special requests
- And several other booking-related features.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📊 Project Workflow

### 1. Data Loading

- Import dataset using Pandas
- Inspect dataset dimensions
- View summary statistics
- Check data types

---

### 2. Data Cleaning

The notebook performs preprocessing steps such as:

- Handling missing values
- Removing unnecessary columns
- Converting categorical features
- Preparing the dataset for machine learning

---

### 3. Exploratory Data Analysis (EDA)

Several visualizations are created to understand:

- Booking cancellation distribution
- Hotel type analysis
- Customer behavior
- Booking trends
- Feature relationships
- Correlation among numerical variables

---

### 4. Feature Engineering

The notebook prepares the data by:

- Encoding categorical variables using **One-Hot Encoding**
- Scaling numerical features using **MinMaxScaler**
- Splitting the dataset into training and testing sets

---

## 🤖 Machine Learning Models

### 1. Logistic Regression

A baseline classification model trained using:

```python
LogisticRegression(solver='liblinear')
```

---

### 2. Decision Tree Classifier

A Decision Tree model is implemented to capture nonlinear relationships in the data.

---

### 3. Random Forest Classifier

The ensemble model is trained using:

```python
RandomForestClassifier(
    random_state=42,
    n_jobs=-1
)
```

Random Forest provides the best performance among the implemented models.

---

## 📊 Evaluation Metrics

Each model is evaluated using:

- Accuracy Score
- Confusion Matrix
- Precision
- Recall
- F1-Score
- Classification Report

---

## 📈 Results

| Model | Accuracy |
|--------|---------:|
| Logistic Regression | **82.99%** |
| Decision Tree Classifier | **92.82%** |
| Random Forest Classifier | **94.95%** |

**Best Performing Model:** ✅ Random Forest Classifier

---

---

## 🎯 Conclusion

This project demonstrates how machine learning can help hotels anticipate booking cancellations and make data-driven operational decisions. After preprocessing, feature engineering, and training multiple classification models, the **Random Forest Classifier** achieved the highest accuracy of **94.95%**, making it the most effective model for predicting hotel booking cancellations in this project.

---

## 👤 Author

**Bindu**

Machine Learning Enthusiast | Deep Learning | NLP | Data Science

---

## 📜 License

This project is intended for educational and learning purposes.
