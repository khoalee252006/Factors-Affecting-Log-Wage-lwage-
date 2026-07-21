[README.md](https://github.com/user-attachments/files/30240240/README.md)
# Factors Affecting Log Wage: Regression Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Regression-brightgreen)

## 📌 Project Overview
This project investigates the key factors that influence the natural logarithm of hourly wage (`lwage`) using a dataset of demographic and educational variables. We perform an end-to-end data analysis workflow, including Exploratory Data Analysis (EDA), statistical testing (ANOVA), and several Machine Learning regression models (OLS, Ridge, Lasso) to predict wages and understand the significance of different predictors.

## 📊 Dataset Description
The dataset (`wage.xlsx`) contains information on 3,010 individuals. 
- **Target Variable**: `lwage` (Log hourly wage)
- **Key Features**:
  - `educ`: Years of education
  - `exper`, `expersq`: Years of experience and its square
  - `IQ`, `KWW`: Cognitive test scores
  - Demographic indicators: `black`, `married`, `south`, `smsa` (Urban)
  - Parents' education: `fatheduc`, `motheduc`

*Note: Missing values in several columns (like IQ, parents' education) were handled appropriately during data preprocessing.*

## 📁 Repository Structure
```text
.
├── figures/                   # Visualizations and plots generated from the notebook
├── Project_1_Final.ipynb      # Main Jupyter Notebook containing all code, EDA, and models
├── Project 1.pdf              # Detailed project report / presentation slides
├── wage.xlsx                  # Raw dataset used for analysis
└── README.md                  # Project documentation (this file)
```

## 🛠️ Methods & Technologies Used
- **Data Processing**: `pandas`, `numpy`
- **Visualization**: `matplotlib`, `seaborn`
- **Statistical Analysis**: `statsmodels`, `scipy` (ANOVA, VIF, Durbin-Watson)
- **Machine Learning**: `scikit-learn` (Linear Regression, Ridge, Lasso, Cross-Validation)

## 🚀 How to Run the Project
1. **Clone the repository**:
   ```bash
   git clone https://github.com/khoalee252006/Factors-Affecting-Log-Wage-lwage-.git
   cd Factors-Affecting-Log-Wage-lwage-
   ```
2. **Install required libraries**:
   Ensure you have Python installed, then install the dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn statsmodels scipy openpyxl
   ```
3. **Run the Notebook**:
   Open Jupyter Notebook or Jupyter Lab and run `Project_1_Final.ipynb`:
   ```bash
   jupyter notebook Project_1_Final.ipynb
   ```

## 📈 Key Findings
- **Education & Experience**: Both have a significant positive impact on wage. Experience exhibits an inverted-U shape relationship (wages peak after a certain number of years of experience).
- **Cognitive Skills**: Higher IQ and KWW (Knowledge of the World of Work) scores are strongly correlated with higher wages.
- **Demographics**: Being in an urban area (SMSA) is associated with a wage premium, whereas living in the South or being Black is associated with a wage penalty in the dataset.
- **Model Performance**: The extended regression models (including Ridge and Lasso) provided stable predictions, effectively handled potential multicollinearity, and explained a significant portion of the wage variation.

## ✍️ Author
- **[Lê Ngọc Khoa]** - [khoalee252006](https://github.com/khoalee252006)
- **[Trần Phú Tân]**

---
*This project was completed as part of the MAI391 (Mathematics for Machine Learning) coursework at FPT University.*
