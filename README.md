📂 Repository Structure
saas-churn-prediction/
│── data/
│   └── saas_churn_data.csv     # dataset (optional, or link in README)
│
│── notebook/
│   └── saas_churn_analysis.ipynb   # your Google Colab notebook
│
│── src/
│   ├── preprocessing.py        # data cleaning & encoding functions
│   ├── train.py                # model training with CV
│   ├── evaluate.py             # metrics & reporting
│
│── results/
│   ├── confusion_matrix.png    # confusion matrix plot
│   ├── roc_curve.png           # ROC curve plot
│   └── metrics_report.txt      # full evaluation report
│
│── README.md                   # project documentation
│── requirements.txt            # Python dependencies

# Evaluate-ML-Models-using-Cross-Validation-and-Advanced-Metrics-Precision-Recall-F1-score-

This project focuses on predicting **customer churn** for a SaaS company using **Machine Learning**.  
We evaluate models with **Cross-Validation, Precision, Recall, F1-score, Accuracy, and ROC-AUC** to ensure reliability.

---

## 🚀 Features
- Preprocessed SaaS churn dataset with categorical and numerical features.
- Implemented **Stratified K-Fold Cross-Validation**.
- Compared **RandomForestClassifier** and **LogisticRegression**.
- Used **advanced metrics**: Precision, Recall, F1-score, Accuracy, ROC-AUC.
- Visualized **Confusion Matrix & ROC Curve**.
- Modular code: `preprocessing.py`, `train.py`, `evaluate.py`.

---

## 📂 Dataset
- **Rows:** 1000  
- **Columns:** 6  
- **Features:**  
  - `logins_per_week` (numeric)  
  - `time_spent_hours` (numeric)  
  - `support_tickets` (numeric)  
  - `subscription_plan` (categorical)  
  - `payment_history` (categorical)  
  - `churn` (target: 0 = active, 1 = churned)

---

## 🛠 Setup & Installation
```bash
git clone https://github.com/your-username/saas-churn-prediction.git
cd saas-churn-prediction
pip install -r requirements.txt

▶️ Usage

Run the notebook in Google Colab:

Upload dataset to data/.

Open notebook/saas_churn_analysis.ipynb.

Run all cells to reproduce results.

📊 Results

RandomForest: Higher recall (better at catching churners).

Logistic Regression: More interpretable but lower recall.

📌 Sample Metrics (5-Fold CV):

Accuracy: ~68%

Precision: ~29%

Recall: ~10%

F1-score: ~15%

📈 Visualizations

✅ Confusion Matrix

✅ ROC Curve

✅ Classification Report

📌 Deliverables

Full Jupyter Notebook (notebook/saas_churn_analysis.ipynb)

Modular Python scripts (src/)

Evaluation plots (results/)

README.md and requirements.txt

🤝 Credits

Project developed as part of Ezitech Community Internship Program.


---

## 📄 requirements.txt

```txt
pandas
numpy
scikit-learn
matplotlib
seaborn
