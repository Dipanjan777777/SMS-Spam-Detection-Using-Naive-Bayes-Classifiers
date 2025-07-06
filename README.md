# 📩 SMS Spam Detection Using Machine Learning

## 🧠 Problem Statement

In the era of digital communication, **spam messages** are a significant problem that can mislead users, waste time, and sometimes result in financial loss or security threats. The objective of this project is to build a **Machine Learning-based model** that can **accurately classify SMS messages** as either:

- **Spam** (unwanted, malicious, or promotional content)
- **Ham** (genuine messages)

This project utilizes **Natural Language Processing (NLP)** techniques and supervised learning algorithms to detect spam in text messages.

---

## 📊 Project Overview

This notebook-based project performs:

1. **Data Cleaning & Preprocessing**
2. **Text Feature Extraction using CountVectorizer/TF-IDF**
3. **Model Building** using algorithms like Naive Bayes, Logistic Regression, etc.
4. **Model Evaluation** through accuracy, precision, recall, and F1-score
5. **Visualization** including word clouds and confusion matrices

---

## 📁 Dataset Description

The dataset used is the [UCI SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection).  
It contains **5,574** SMS messages labeled as:

- `spam` — spam message  
- `ham` — legitimate (non-spam) message  

Each message is a single line of text with a corresponding label.

---

## ⚙️ Environment Setup with Conda

Follow the steps below to run the project in a **Conda environment**.

### 📦 Step 1: Install Anaconda or Miniconda

Download and install:
- [Anaconda](https://www.anaconda.com/products/distribution) (recommended) or
- [Miniconda](https://docs.conda.io/en/latest/miniconda.html)

---

### 🧪 Step 2: Create a Conda Environment

```bash
conda create --name sms-spam-detection python=3.11 -y
conda activate sms-spam-detection
pip install -r requirements.txt