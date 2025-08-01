# PhishGuard 🔐  
**Detection of Phishing URLs using Machine Learning**

![License](https://img.shields.io/badge/license-MIT-blue.svg)  
![Python](https://img.shields.io/badge/python-3.8%2B-blue)  
![ML](https://img.shields.io/badge/ML-XGBoost%2C%20RandomForest%2C%20ANN-orange)

## 🧠 Overview

**PhishGuard** is a machine learning-based solution designed to detect phishing websites by analyzing various URL features. As phishing remains one of the most dangerous forms of cyberattacks exploiting human behavior rather than system vulnerabilities, this project builds a robust detection system using ML models like XGBoost, Random Forest, Decision Tree, and Artificial Neural Networks.

This solution aims to proactively classify suspicious websites based on key indicators in the URL and domain metadata — offering a scalable and automated cybersecurity measure.

---

## 🎯 Objectives

- Detect phishing websites using machine learning algorithms.
- Extract and analyze important URL-based features such as domain length, presence of HTTPS, special characters, etc.
- Evaluate and compare different models to identify the most accurate classifier.
- Deploy the final model using PaaS (e.g., Render) for real-world use.

---

## 📊 Dataset

Five datasets were used and processed:

- `Benign_list_big_final.csv` – Dataset of legitimate websites.
- `online-valid.csv` – Mixed dataset of phishing and legitimate sites.
- `legitimate.csv` – Extracted and cleaned dataset of benign URLs.
- `phishing.csv` – Extracted and cleaned dataset of phishing URLs.
- `urldata.csv` – Balanced dataset combining both phishing and legitimate samples for final model training.

> Feature Count: **13 URL-based features**

---

## 🧪 Methodology

### 🔧 Preprocessing
- Cleaned datasets (removed duplicates, handled missing values).
- Encoded categorical variables (e.g., WHOIS data).
- Feature engineering from URL structure, domain attributes, and user behavior patterns.

### 🧠 Models Used
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- XGBoost
- Multi-Layer Perceptron (MLP)
- Artificial Neural Network (ANN using Keras)

> Hyperparameter tuning was done using **Grid Search** and **Bayesian Optimization**.

### 📈 Evaluation Metrics
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **AUC-ROC**

---

## ☁️ Deployment

The trained model is deployed using **Render (PaaS)**, allowing real-time classification of URLs through a web service interface. This architecture leverages **Cloud GPU resources (Google Colab)** for training and **Render** for hosting.

---

## 🖥️ Tech Stack

- **Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, XGBoost, Keras, TensorFlow, Matplotlib
- **Platform**: Google Colab (training), Render (deployment)
- **Dataset Source**: Public repositories (Kaggle)

---

