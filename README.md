# ☀️ Annual Solar Energy Production Prediction

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR-GITHUB-USERNAME/solar-energy-production-prediction/blob/main/notebooks/solar_energy_pipeline.ipynb)

An end-to-end Machine Learning regression pipeline developed entirely in Google Colab to accurately predict annual solar energy output (kWh) based on hardware capacity dimensions, regional geography tracking, and deployment timeline age metrics.

---

## 📂 Repository Structure
* `notebooks/`: Contains the master, self-contained Google Colab notebook (`solar_annual_energy_pipeline.ipynb`) handling EDA, target encoding maps, multi-model regression pipelines, evaluation metrics, and the interactive deployment CLI.
* `.gitignore`: Configured parameters to maintain a professional workspace clean of hidden local system cache files.

## 🛠️ Data Science Pipeline Highlights
* **Smooth Target Encoding:** Engineered target values with an explicit smoothing factor ($\alpha = 10$) applied on high-cardinality values (`Zip`, `Developer`, `City/Town`) preventing data leakage.
* **Production Validation Framework:** Models are trained using Scikit-Learn `Pipeline` and `ColumnTransformer` modules to guarantee standard scaling operations run securely across validation test states.
* **Architecture Testing:** Evaluates performance across Ridge, Linear Regression, Random Forest, Gradient Boosting, and XGBoost structures simultaneously.

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Processing:** Polars, Pandas, NumPy
* **Machine Learning:** Scikit-Learn, XGBoost
* **Visualizations:** Matplotlib, Seaborn

## 📊 Model Performance Evaluation

The models were evaluated using an 80/20 train-test split. Below are the performance metrics across all tested architectures, sorted by their Root Mean Squared Error (RMSE).

* **Top Performer:** <span style="color: #00FFFF;">Random Forest</span>
* **Accuracy** | **97.43%**
* **Precision** | **95.96%**
* **Recall** | **99.01%**
* **AUC** | **99.75%**


## ⚙️ How to Run the Code Instantly
You do not need to install anything locally on your machine to test this project! 

1. Click the **Open In Colab** badge at the top of this page.
2. If you are using your own dataset, upload your data file using the left-hand folder sidebar menu inside the Colab workspace.
3. Click **Runtime > Run all** in the top menu bar to execute the entire data pipeline and trigger the interactive solar production calculator tool.