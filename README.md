# Fake_News_Classifier
This project is a Machine Learning classifier built to distinguish between **fake** and **real** news articles using **Logistic Regression**. The model is trained on the WELFake dataset and uses **TF-IDF vectorization** for text preprocessing.

---

## Dataset

- **Source**: [WELFake Dataset on Kaggle](https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification)
- **Columns**:
  - `title`: Headline of the news article
  - `text`: Full content of the article
  - `label`: 1 = Fake, 0 = Real

---
## Model Overview

| Step | Description |
|------|-------------|
|  Data Cleaning | Removed noise, nulls, and combined `title` + `text` |
|  Preprocessing | Text normalized and cleaned using regex |
|  Feature Extraction | Used `TfidfVectorizer` to convert text to numerical vectors |
|  Model Training | Logistic Regression on 80/20 split |
|  Evaluation | Accuracy, Classification Report, and Confusion Matrix |

---
##  Results

- **Accuracy**: ~90%+
- **Evaluation**: Precision, Recall, F1-Score
- **Confusion Matrix**:
  - True Positives: Correctly identified Fake News
  - True Negatives: Correctly identified Real News

---
##  Tech Stack

- Python
- Pandas, NumPy
- scikit-learn
- NLTK
- Matplotlib (for confusion matrix)
- Google Colab

---
