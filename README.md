# Credit Card Fraud Detection

This project builds and evaluates machine learning models to detect fraudulent credit card transactions using a highly imbalanced real-world dataset. The focus is on proper data preprocessing, handling class imbalance, and evaluating models with metrics that matter for fraud detection such as recall and ROC-AUC.

---

## 📌 Project Overview

Credit card fraud detection is a challenging classification problem due to:
- Extreme class imbalance (fraudulent transactions are very rare)
- High cost of false negatives (missed fraud cases)
- Need for careful model evaluation beyond simple accuracy

This project implements an end-to-end machine learning pipeline including:
- Exploratory Data Analysis (EDA)
- Feature scaling and transformation
- Model training and comparison
- Handling class imbalance using oversampling techniques
- Performance evaluation using ROC curves and confusion matrices

---

## 📊 Dataset

The dataset used in this project is publicly available on **:contentReference[oaicite:0]{index=0}**:

🔗 **Credit Card Fraud Dataset**  
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?resource=download

### Dataset Details
- Transactions made by European cardholders
- Features are anonymized using PCA (`V1`–`V28`)
- `Time` and `Amount` are not transformed
- Target variable:
  - `Class = 0` → Non-fraudulent transaction  
  - `Class = 1` → Fraudulent transaction

⚠️ **Note:**  
The dataset is **not included in this repository** due to GitHub file size limitations.  
After downloading, place the dataset in a local `data/` directory.

Example:
```text
data/
└── creditcard.csv
