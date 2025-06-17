# 📧 Spam vs. Ham Email Classifier

This project is a **machine learning-based email classifier** that distinguishes between **spam** and **ham (non-spam)** emails using natural language processing (NLP). It uses **TF-IDF vectorization**, **SMOTE** for class balancing, and a **Naive Bayes** classifier.

---

## 📌 Project Overview

- 📂 **Dataset**: `spam_ham_dataset.csv`  
- 🧠 **Model**: Multinomial Naive Bayes  
- 🔤 **Text Processing**: TF-IDF Vectorization  
- ⚖️ **Class Balancing**: SMOTE (Synthetic Minority Oversampling Technique)  
- 📊 **Visualization**: Matplotlib & Seaborn  
- 📈 **Metrics**: Accuracy, Confusion Matrix, Classification Report

---

## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| Python | Programming language |
| Pandas / NumPy | Data manipulation |
| Matplotlib / Seaborn | Data visualization |
| Scikit-learn | ML algorithms & preprocessing |
| imbalanced-learn (SMOTE) | Handle class imbalance |
| TF-IDF | Convert text to numeric vectors |
| Naive Bayes | Spam detection model |

---

## 📊 Workflow

1. **Data Preprocessing**
   - Drop unnecessary columns
   - Encode labels (`ham` = 0, `spam` = 1)
   - Handle class imbalance using SMOTE

2. **Text Vectorization**
   - Apply `TfidfVectorizer` to transform email text

3. **Model Training**
   - Train a `MultinomialNB` model on vectorized, balanced data

4. **Evaluation**
   - Use Accuracy, Precision, Recall, F1-Score
   - Plot Confusion Matrix & Classification Heatmap

5. **Real-world Predictions**
   - Predict custom emails like:
     - `"Limited-time offer on weight loss pills"`
     - `"Your resume is shortlisted for the AI internship"`

## 📈 Evaluation

- ✅ **Accuracy**: ~97.2%
- 📚 **Classification Report** (
-                               precision    recall  f1-score   support

                    Ham (0)       0.99      0.97      0.98       742
                   Spam (1)       0.94      0.97      0.95       293

                   Accuracy                           0.97      1035
                  Macro Avg       0.96      0.97      0.97      1035
                  Weighted Avg       0.97      0.97      0.97      1035

- 🔢 **Confusion Matrix**(
-       [[723,  19],
        [ 10, 283]], dtype=int64))
