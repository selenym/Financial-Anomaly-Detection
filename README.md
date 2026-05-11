# Financial Anomaly Detection: Machine Learning vs. Rule-Based Systems
This repository contains a comprehensive study on detecting fraudulent credit card transactions by comparing traditional rule-based systems with modern machine learning approaches (Random Forest and XGBoost).

# 📌 Project Overview
Fraud detection is critical in the digital economy to prevent billions of dollars in losses and maintain customer trust. Traditional systems rely on static, expert-defined rules that often fail to adapt to evolving fraud patterns, leading to high false-positive rates. This project demonstrates how data-driven "Pattern of Life" analysis can overcome these limitations.

# 📊 Dataset & Methodology
Dataset: Kaggle's "Credit Card Fraud Detection" dataset, containing 284,807 transactions by European cardholders.

Imbalance Handling: The dataset is highly imbalanced (only 0.172% are frauds). SMOTE (Synthetic Minority Over-sampling Technique) was used to balance the training data.

Features: Variables are PCA-transformed for privacy, with 'Time' and 'Amount' remaining in their original form.

# 🚀 Performance Comparison
We evaluated three different approaches. The results highlight the massive leap in detection capability provided by Machine Learning:

<img width="650" height="100" alt="image" src="https://github.com/user-attachments/assets/e81104fb-04cb-46d2-8222-a3f46813ac5b" />
   
# 📈 Key Insights
Random Forest emerged as the top performer with a 0.97 AUC, showing superior robustness in distinguishing between legitimate and fraudulent transactions.

While the rule-based system achieved a misleading 99% accuracy, its Recall was only 2%, meaning it missed almost all fraud. Machine Learning pushed this detection rate to over 80%.

The models successfully identified "Micro-structuring" patterns (small, frequent anomalies) that static rules typically ignore.

<img width="527" height="393" alt="image" src="https://github.com/user-attachments/assets/8f4f52dd-726e-4ec4-aad4-8b44a8077ab8" />


<img width="527" height="400" alt="image" src="https://github.com/user-attachments/assets/82f47a20-77d4-4887-a0f7-c2e6f1e88264" />

# 🛠️ Tech Stack
Language: Python

Libraries: Pandas, NumPy, Scikit-Learn, XGBoost, Matplotlib, Seaborn

Tools: Jupyter Notebook / Google Colab

# ⚠️ Limitations & Future Work
Explainability: While Random Forest offers high accuracy, it acts more as a "black box" compared to simple IF-THEN rules. Future work involves integrating SHAP or LIME for better model interpretability.

Advanced Architectures: Exploring Deep Learning (Autoencoders) and Graph Neural Networks (GNNs) to detect complex money laundering networks.
