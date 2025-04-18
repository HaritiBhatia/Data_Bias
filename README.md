# Understanding and Mitigating Data Bias in Machine Learning and Data Science

## 📌 Project Overview

This project explores how **data bias** impacts machine learning models, with a focus on **selection bias** and **demographic imbalance**, particularly in socially sensitive domains like **loan approvals**. It evaluates mitigation strategies such as **SMOTE**, **random oversampling**, and **propensity score matching (PSM)** to promote fairness and equitable model performance.

---

## 📊 Dataset

**Source**: `Bank-Loan.csv`  
The dataset includes demographic and financial details for loan applicants, with the target column indicating loan approval status.

**Key Columns:**
- `Age`
- `Gender`
- `Income`
- `Employment Status`
- `Credit Score`
- `Loan Amount`
- `Loan Approved`

**Bias Identified:**
- Gender imbalance: ~82% Male
- Approval Rate Disparity: Males favored
- Class imbalance: 69% approved vs. 31% denied loans

---

## 🧠 Problem Statement

- **Issue**: Underrepresentation of certain demographic groups (e.g., women, part-time workers) and skewed loan approval outcomes.
- **Goal**: Detect and mitigate bias to ensure fairer predictions across demographic groups.

---

## 🧪 Methodology

### 1. Exploratory Data Analysis (EDA)
- Identified class imbalance and demographic disparities
- Visualized loan approvals by gender, income levels, etc.

### 2. Data Preprocessing
- Missing value imputation using median/mode
- Label encoding for categorical variables
- Outlier detection and feature scaling

### 3. Bias Mitigation Techniques
- **Random Oversampling**: Balanced gender distribution
- **SMOTE**: Balanced approval class distribution
- **Propensity Score Matching (PSM)**: Compared loan approval outcomes between matched groups with similar profiles

---

## ⚙️ Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Imbalanced-learn (`SMOTE`)
- Jupyter Notebook

---

## 📈 Results

- **Before Mitigation**: Significant demographic and class bias
- **After Mitigation**:
  - Balanced class and gender representation
  - Reduced gender-based prediction bias
  - Improved model fairness and generalization

---

## 📚 Key Takeaways

- Bias can emerge from unbalanced demographic or historical data.
- Techniques like **SMOTE**, **resampling**, and **fairness-aware algorithms** improve equity in model predictions.
- Regular auditing and fairness metrics (e.g., Demographic Parity) are essential.

---

## 📄 Files

- `Group_26_Data_Bias.ipynb`: Jupyter Notebook for the analysis and modeling
- `Bank-Loan.csv`: Raw dataset used in the project
- `Group26_Data_Bias.pdf`: Final report with methodology, visualizations, and results
- `Data_Bias_Latex_source.zip`: Source files for the LaTeX report
