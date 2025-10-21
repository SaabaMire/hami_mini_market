#  Spam Email Classifier - HamiSkills Machine Learning Track (Week 1)

##  Author
**Sabirin Mire Abukar**  
HamiSkills Internship – Machine Learning Track  

---

##  Project Overview
This project builds a **Spam Email Classifier** for *Hami MiniMarket* to automatically detect whether incoming emails are **Spam** or **Ham (Not Spam)**.

It is part of the **HamiSkills Week 1 Machine Learning Track** task, focusing on text preprocessing, feature extraction using **TF-IDF**, and model training using **Scikit-learn**.

---

##  Dataset
- **Source:** UCI SMS Spam Collection Dataset  
  [🔗 Dataset Link](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)  
- **Description:** Contains labeled email messages as either *spam* or *ham*.  
- **Columns:**
  - `Category`: Spam (0) or Ham (1)
  - `Message`: Free entry in 2 a wkly comp to win FA Cup final tkts 21st May 2005. Text FA to 87121 to receive entry question(std txt rate)T&C's apply 08452810075over18's or WHO ARE YOU SEEING?

---

##  Technologies Used
- Python 3.13.7
- Pandas & NumPy  
- Scikit-learn (TF-IDF, Logistic Regression, )  
- Joblib (for model saving)  
- Regex (text cleaning)

---

## Steps in the Project

1. **Data Loading**
   - Loaded dataset using `pandas.read_csv()`.
2. **Preprocessing**
   - Converted all text to lowercase  
   - Removed punctuation and stopwords  
   - Encoded labels (`spam → 0`, `ham → 1`)
3. **Feature Extraction**
   - Used `TfidfVectorizer` to convert text into numerical vectors.
4. **Model Training**
   - Trained both **Logistic Regression** and **Naive Bayes** models.
5. **Model Evaluation**
   - Evaluated performance using:
     - Accuracy
     - Precision
     - Recall
     - F1 Score
     - Confusion Matrix
6. **Model Saving**
   - Saved the trained model and vectorizer using `joblib`.
7. **CLI Prediction Tool**
   - Allows users to input a message and instantly get a spam/ham prediction.

---

## Results

| Model | Accuracy | Precision | Recall | F1 Score |
|--------|-----------|------------|----------|-----------|
| Logistic Regression | ~96% | ~100% | ~72% | ~84% |




---




