# Machine-Learning-In-Java

This repository contains simple implementations of **Linear Regression** and **Logistic Regression** written completely from scratch in Java, without using any external machine learning libraries.

## 🚀 Overview

The goal of this project is to understand the internal workings of machine learning algorithms by implementing them manually using core Java concepts like:

* Interfaces
* Classes
* Arrays
* Gradient Descent

The project demonstrates:

* Regression (predicting continuous values)
* Classification (binary classification)
* Model evaluation
* Train-test splitting

---

## 🧠 Models Implemented

### 1. Linear Regression

* Predicts continuous values (e.g., student marks)
* Uses **gradient descent**
* Outputs rounded predictions

### 2. Logistic Regression

* Binary classification (Pass/Fail)
* Uses **sigmoid function**
* Outputs class labels (0 or 1)

---

## 📂 Project Structure

```
.
├── Model.java        # Contains all classes (Model, LinearRegression, LogisticRegression, Main)
├── Pass-Fail Data.csv
└── README.md
```

---

## ⚙️ How It Works

1. Reads dataset from CSV file
2. Splits data into:

   * 80% training
   * 20% testing
3. Trains both models
4. Evaluates performance on test data

---

## 🧪 Sample Output

### Logistic Regression

```
Accuracy of logistic on testing set 100.0%
```

✔ Perfect classification on the test set

---

### Linear Regression

```
Predicted: 88 -> Observed: 88
Predicted: 60 -> Observed: 55
...
Accuracy of linear on testing set 15.0%
```

* Shows prediction vs actual values
* Lower accuracy due to regression rounding + dataset nature

---

## 📊 Observations

* Logistic Regression performed extremely well (100% accuracy)
* Linear Regression struggled due to:

  * Treating classification-like data as continuous
  * Rounding predictions to integers
* Dataset likely favors classification more than regression

---

## 🛠️ How to Run

### Compile

```
javac Model.java
```

### Run

```
java Main
```

---

## ⚠️ Common Errors

### ❌ Wrong file extension

```
javac Model.jav
```

✔ Fix:

```
javac Model.java
```

---

### ❌ Variable not found

```
cannot find symbol y_pred / y_test
```

✔ Fix:

* Ensure correct variable names (`Y_pred`, `Y_test`)
* Java is case-sensitive

---

## 📈 Possible Improvements

* Add feature scaling (normalization)
* Use double instead of int for better precision
* Implement:

  * Mean Squared Error (MSE)
  * Confusion Matrix
* Add support for multi-class classification
* Improve train-test split randomness

---

## 🎯 Learning Outcomes

This project helps in understanding:

* How gradient descent updates weights
* Difference between regression and classification
* Importance of data preprocessing
* Model evaluation techniques

---

## 📌 Author

Your Name

---

## ⭐ If you like this project

Give it a star ⭐ and feel free to contribute!
