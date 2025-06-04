# 🌱 Renewable Energy ESG Modeling

This project uses machine learning to identify how **Environmental, Social, and Governance (ESG)** factors influence renewable energy adoption across countries. Developed as part of an academic assignment, the project showcases skills in data cleaning, feature engineering, and advanced regression modeling.

---

## 🎯 Objective

- Understand which ESG indicators are most predictive of **renewable energy consumption** (% of total energy use).
- Predict renewable energy adoption using robust regression models.
- Provide **data-driven recommendations** for governments and sustainability investors.

---

## 🧪 Machine Learning Workflow

- **Data Source**: World Bank Open Data (manually compiled)
- **Target Variable**: Renewable energy consumption (% of total energy)
- **Key Features**:
  - Access to electricity
  - Rule of Law Index
  - Clean fuels and cooking
  - Energy use per GDP
  - Female labor force participation
- **Preprocessing**:
  - Forward/backward fill for missing values
  - Scaled with `StandardScaler`
  - Correlation check for multicollinearity

### 📈 Models Used

| Model          | MAE   | MSE    | R² Score |
|----------------|-------|--------|----------|
| **XGBoost**    | 4.12  | 42.39  | 0.9486   |
| **RandomForest** | 3.66 | 42.92  | 0.9479   |

- Residual analysis confirmed minimal overfitting.
- Feature importance graphs were used for interpretability.

---

## 📊 Key Insights (From Final Report)

- **Access to clean fuels** and **strong rule of law** are consistently associated with higher renewable energy use.
- Countries with **better governance scores** (e.g., corruption control, legal frameworks) are more sustainable.
- **Agricultural intensity** has a mixed effect, likely due to varying levels of modernization.
- **Digital access** and **female workforce participation** emerged as moderate influencers.

---

## 📁 Repository Structure

enewable-energy-esg-modeling/
├── data/
│ ├── ESG_Data.csv # Final feature-engineered dataset
│ └── README.md # Description of variables and source
├── notebooks/
│ └── esg_modelling_notebook.ipynb
├── visuals/
│ └── esg_plot_1.png → esg_plot_5.png
├── README.md
└── requirements.txt

---

## 🔧 Tools Used

- Python (pandas, seaborn, scikit-learn, xgboost)
- Jupyter Notebook
- World Bank Data API

---

## 📌 Recommendations

- Prioritize investments in countries with high legal stability and fuel accessibility.
- Tailor policy based on digital, social, and energy usage metrics.
- Use model retraining yearly with updated economic data.

---

## 👤 Author

**Don Richardson Bayya**  
