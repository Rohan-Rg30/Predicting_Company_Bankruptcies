# 🏢 Company Bankruptcy Prediction Pipeline

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Rohan-Rg30/Predicting_Company_Bankruptcies/blob/main/Notebook/Predicting_Company_Bankruptcies.ipynb)

An end-to-end Machine Learning binary classification pipeline developed entirely in Google Colab to accurately predict company bankruptcies based on high-dimensional financial ratios, automated class-balancing techniques, and a soft-voting tuned ensemble model.

---

## 📂 Repository Structure
* `notebooks/`: Contains the master, self-contained Google Colab notebook (`Predicting_Company_Bankruptcies.ipynb`) handling EDA, automated feature selection, class rebalancing, multi-model classification benchmarks, and threshold optimization.
* `.gitignore`: Configured parameters to maintain a professional workspace clean of hidden local system cache files.

## 🛠️ Data Science Pipeline Highlights
* **Automated Feature Selection:** Utilizes ANOVA F-Scores (`SelectKBest`) to automatically filter and extract the top 25 most mathematically significant predictors from 96 baseline financial attributes.
* **Robust Imbalance Mitigation:** Combines Synthetic Minority Over-sampling Technique with Tomek Links (`SMOTETomek`) to flawlessly balance an initial 1:30 heavily skewed class ratio (6,599 healthy vs. 220 bankrupt firms).
* **Tuned Soft-Voting Ensemble:** Combines Random Forest, Gradient Boosting, and Support Vector Machine structures simultaneously via a custom-weighted `VotingClassifier` (weights 2:2:1) paired with custom threshold optimization to maximize financial risk identification.

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Processing:** Imbalanced-Learn, Pandas, NumPy
* **Machine Learning:** Scikit-Learn (Ensembles, SVM, Neighbors)
* **Visualizations:** Matplotlib, Seaborn

## 📊 Baseline Model Performance Benchmark

The tested architectures were evaluated using an 80/20 train-test split. Below are the performance metrics across all standalone algorithms, sorted by their predictive performance:

* **Top Performer:** <span style="color: #00FFFF;">Random Forest</span>
* **Accuracy** | **97.27%**
* **Precision** | **96.36%**
* **Recall** | **98.26%**
* **AUC** | **99.53%**

## ⚙️ How to open the Code Instantly
You do not need to install anything locally on your machine to test this project! 

* Click the **Open In Colab** badge at the top of this page.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to check the [issues page](https://github.com/Rohan_Rg30/Predicting_Hotel_Reservation_Cancellations/issues) or open a pull request.

## 📜 License

**© Spinnaker Analytics**. All rights reserved.
This project was assigned as part of an on-the-job training program at Spinnaker Analytics and is the property of Spinnaker Analytics. It is shared publicly on GitHub for portfolio/demonstration purposes only. No part of this code, dataset pipeline, or documentation may be copied, redistributed, or used commercially without written permission from Spinnaker Analytics.

## 🙋 Author

**Rohan Gaikwad — Data Scientist**

[LinkedIn](https://www.linkedin.com/in/rohan-gaikwad-8b1976418)

Project completed as part of a 6-month Data Science training program at **Spinnaker Analytics**.

---
<p align="center">⭐ If you found this project useful, consider giving it a star!</p>
