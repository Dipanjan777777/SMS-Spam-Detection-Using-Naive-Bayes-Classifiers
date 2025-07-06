# 📩 SMS Spam Detection Using Naive Bayes Classifiers

## 📌 Problem Statement

Spam SMS messages can clutter inboxes, waste time, and pose serious security threats. The goal of this project is to build an efficient text classification system that can automatically detect whether an SMS message is **spam** or **ham** (not spam), using **machine learning** and **natural language processing (NLP)** techniques.

---

## 🧠 Algorithms Used

This project experiments with three types of **Naive Bayes classifiers**:

1. **Multinomial Naive Bayes**  
2. **Bernoulli Naive Bayes**  
3. **Gaussian Naive Bayes**

Each of them is trained and evaluated using accuracy and precision metrics.

---

## 🎯 Model Performance

| Model                    | Accuracy (Test Set) |
|-------------------------|---------------------|
| Multinomial Naive Bayes | ✅ 97.95%            |
| Bernoulli Naive Bayes   | ✅ 96.66%            |
| Gaussian Naive Bayes    | ✅ 81.97%            |

> ✅ **Best Performing Model:** Multinomial Naive Bayes  
> It achieved the **highest accuracy of 97.95%** on the test data.

---

## 📂 Dataset

This project uses the **[SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)** from Kaggle.

### 🧾 Dataset Details:
- **Total samples:** 5,574 SMS messages  
- **Columns:**
  - `v1` – Label: `ham` (genuine) or `spam` (unwanted)
  - `v2` – SMS message text
- **Preprocessing:**
  - Dropped unnecessary columns: `Unnamed: 2`, `Unnamed: 3`, `Unnamed: 4`
  - Renamed:
    - `v1` → `target`
    - `v2` → `text`
  - Encoded labels: `ham` = 0, `spam` = 1

---

## 🧼 Data Preprocessing

Steps included:

1. Lowercasing text
2. Removing punctuation and special characters
3. Removing stopwords using NLTK
4. Stemming with `PorterStemmer`
5. Encoding target labels using `LabelEncoder`
6. Vectorization using `TF-IDF`

---

## ⚙️ Environment Setup (with Conda)

Follow the instructions to set up and run the project locally.

### 1️⃣ Install Conda
Get [Anaconda](https://www.anaconda.com/products/distribution) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).

### 2️⃣ Create and Activate Environment

```bash
conda create --name sms-spam-detection python=3.9 -y
conda activate sms-spam-detection
pip install -r requirements.txt