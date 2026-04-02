# 📧 Spam Mail Classification System

## 🚀 Project Overview

This repository contains a machine learning project designed to classify email messages as either **Spam** or **Ham (non-spam)** using **Python** and **Logistic Regression**.

The system processes text-based email data, converts it into numerical features using **TF-IDF Vectorization**, and applies a Logistic Regression model to predict the category of new, unseen messages.

---

## 🛠️ Technical Stack

* **Language:** Python 3
* **Data Analysis:** pandas, numpy
* **Machine Learning:** scikit-learn
* **Environment:** Jupyter Notebook / Google Colab

---

## 📊 Dataset Specifications

The model is trained on a dataset containing **5,572 entries** with two primary columns:

* **Category:** The label (Spam or Ham)
* **Message:** The raw text content of the email

---

## ⚙️ Workflow

### 1. Data Pre-processing

* Load data from `mail_data.csv`
* Handle null values by replacing them with empty strings

### 2. Label Encoding

* Spam → **0**
* Ham → **1**

### 3. Feature Extraction

* Uses **TfidfVectorizer** to convert text into numerical features
* Parameters:

  * `min_df=1`
  * `stop_words='english'`
  * `lowercase=True`

### 4. Model Training

* **Algorithm:** Logistic Regression
* **Data Split:** 80% Training, 20% Testing

---

## 📈 Performance

The model achieves high accuracy:

* **Training Accuracy:** ~96.77%
* **Test Accuracy:** ~96.68%

---

## 💻 How to Use

### 1. Prerequisites

Install required libraries:

```bash
pip install numpy pandas scikit-learn
```

### 2. Data Setup

* Place your `mail_data.csv` file in the project directory
* Ensure it contains the following columns:

  * `Category`
  * `Message`

### 3. Run the Project

* Open the Jupyter Notebook or Google Colab
* Run all cells to train and test the model

---

## 📌 Future Improvements

* Deploy as a web application (Flask/Django)
* Use advanced models (LSTM, BERT)
* Improve dataset size and diversity
* Add real-time spam detection

---

