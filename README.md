# student-academic-stress-classification
Machine Learning project using Random Forest to classify student academic stress levels (low, medium, high) based on Kaggle dataset.
🎓 Student Academic Stress Classification
## 📌 Project Overview
This project explores **student academic stress** using a Kaggle dataset.
We built a **Random Forest model** to classify stress levels into categories:
* **Low Stress** (1–2)
* **Medium Stress** (3)
* **High Stress** (4–5)
The goal is to understand **which factors contribute most** to academic stress and evaluate how well machine learning can predict stress levels.

## 📊 Dataset
* **Source**: [Student Academic Stress Dataset (Kaggle)](https://www.kaggle.com/datasets/poushal02/student-academic-stress-real-world-dataset/data)
* **Features**:
  * Academic Competition
  * Peer Pressure
  * Academic Pressure from Home
* **Target**: Stress Level (1–5)

## 🧠 Model
* Algorithm: **Random Forest Classifier**
* Data split: Train/Test
* Metrics: Accuracy, Precision, Recall, F1-score
* Visualization: Confusion Matrix

## 🔍 Results
### Classification Report
* **Accuracy**: \~53%
* **Low Stress**: Recall = 100% (all low stress detected correctly)
* **Medium Stress**: Model struggles, recall = 0% (class imbalance issue)
* **High Stress**: Precision & Recall = 67%

### Confusion Matrix
![Confusion Matrix](confusion_matrix.png)
### Feature Importance
* Academic Competition → **42%**
* Peer Pressure → **31%**
* Academic Pressure (Home) → **27%**

## ✅ Key Insights
* Model works best at separating **low** and **high stress**.
* **Medium stress** is harder to predict (likely due to fewer samples).
* **Academic competition** is the biggest factor influencing stress.

## 🚀 How to Run

```bash
# clone repo
git clone https://github.com/username/student-stress-classification.git
cd student-stress-classification

# install dependencies
pip install -r requirements.txt

# run notebook
jupyter notebook
```
## 📌 Future Improvements

* Handle **class imbalance** (SMOTE, oversampling, etc.)
* Try other models (XGBoost, SVM, Neural Networks)
* Collect more balanced data for medium stress cases

## 📎 References

* Kaggle Dataset: [Student Academic Stress Dataset](https://www.kaggle.com/datasets/poushal02/student-academic-stress-real-world-dataset/data)
