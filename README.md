# Applied-project
Applied Project - Order Risk Prediction
# 📦 DataCo Supply Chain – Late Delivery Risk Prediction

## 📌 Project Overview

Late deliveries are a major challenge in supply chain management, affecting customer satisfaction, operational efficiency, and business performance.

This project uses **Machine Learning techniques to predict late delivery risk** based on order details available before shipment. The objective is to help businesses identify potentially delayed orders early and make better supply chain decisions.

The project uses the DataCo Smart Supply Chain dataset and compares multiple classification algorithms to identify an effective predictive model.

## 🎯 Project Objectives

- Analyse historical supply chain and order data.
- Identify factors associated with late deliveries.
- Perform Exploratory Data Analysis (EDA).
- Engineer meaningful features from order information.
- Build and compare multiple Machine Learning classification models.
- Evaluate model performance using classification metrics.
- Predict whether a new order is likely to be delivered late or on time.

## 🛠️ Technologies & Tools

- **Programming Language:** Python
- **Data Analysis:** Pandas, NumPy
- **Data Visualisation:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn, XGBoost
- **Development Environment:** Jupyter Notebook
- **Dataset:** Kaggle – DataCo Smart Supply Chain Dataset

## 📊 Dataset

The project uses the [DataCo Smart Supply Chain Dataset](https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis).

The dataset contains approximately 180,000 order records with information about:

- Order details and product information
- Shipping modes and shipment schedules
- Customer segments
- Markets and geographical regions
- Sales and discount information
- Late delivery risk indicators

**Target Variable:** `Late_delivery_risk`

- `0` – Order delivered on time
- `1` – Order at risk of late delivery

## 🔍 Project Workflow

### 1. Data Cleaning & Preparation
- Handled missing values.
- Removed unnecessary identifiers and personal information.
- Removed post-delivery information to prevent data leakage.
- Encoded categorical variables.
- Prepared the dataset for machine learning.

### 2. Exploratory Data Analysis (EDA)
- Analysed late delivery patterns.
- Examined delivery risk across shipping modes.
- Compared markets and geographical regions.
- Investigated scheduled shipping days.
- Analysed monthly and weekly delivery patterns.

### 3. Feature Engineering

Created additional features to improve prediction, including:

- Order year, month, day and hour.
- Weekend and holiday-season indicators.
- Order value.
- Large-order indicators.
- High-value order indicators.
- Discount-related features.

### 4. Machine Learning Models

Implemented and compared five classification algorithms:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Gradient Boosting
5. XGBoost

### 5. Model Evaluation

Evaluated the models using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

Also generated confusion matrices, ROC curves and feature importance visualisations.

## 📈 Results & Key Findings

**XGBoost achieved the best overall performance in the model comparison.**

Approximate evaluation results:

| Metric | XGBoost |
|---|---:|
| ROC-AUC | 0.81 |
| F1-Score | 0.71 |
| Precision | 0.84 |
| Recall | 0.62 |

### Key Business Insights

- Scheduled shipping days and shipping mode were the most influential features.
- Shipping strategy plays an important role in delivery risk.
- Precision was relatively high, while recall indicated opportunities to improve the detection of late orders.
- Removing data leakage was essential to ensure realistic model evaluation.

## 💡 Business Value

This predictive approach can help supply chain and logistics teams:

- Identify potentially delayed orders before shipment.
- Prioritise high-risk orders for monitoring.
- Improve shipping and operational planning.
- Support proactive decision-making.
- Reduce the impact of late deliveries on customer satisfaction.

## 🚀 Future Improvements

- Hyperparameter tuning using GridSearchCV.
- Cross-validation for more robust model evaluation.
- SHAP-based model explainability.
- Threshold optimisation to improve late-delivery detection.
- Development of an interactive prediction dashboard using Streamlit.

## 📂 Repository Structure

```text
Applied-project/
│
├── README.md
├── DataCoOrderRiskPrediction.ipynb
└── Final_Thesis_Submission.docx
```

## ▶️ How to Run the Project

1. Clone this repository:

```bash
git clone https://github.com/akshaireddythota-hue/Applied-project.git
```

2. Navigate to the project directory:

```bash
cd Applied-project
```

3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost kagglehub jupyter
```

4. Open the Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `DataCoOrderRiskPrediction.ipynb` and execute the cells.

**Note:** The dataset is downloaded through KaggleHub when the notebook runs. Ensure you have an internet connection and the required Kaggle access.

---

## 👨‍💻 Author

**Akshai Reddy Thota**

GitHub: [akshaireddythota-hue](https://github.com/akshaireddythota-hue)

---

*This project demonstrates practical applications of Python, Data Analytics, Machine Learning, feature engineering, and predictive modelling in supply chain management.*
