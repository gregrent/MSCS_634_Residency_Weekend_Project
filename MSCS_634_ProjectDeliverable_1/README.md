# Advanced Data Mining for Data-Driven Insights and Predictive Modeling  
## Deliverable 1: Data Collection, Cleaning, and Exploration

---

## 📌 Project Overview

This deliverable focuses on the initial stages of the data mining process, including data collection, data cleaning, and exploratory data analysis (EDA). The objective is to prepare a real-world dataset for advanced data mining tasks by ensuring high data quality and extracting meaningful insights that will guide future predictive modeling.

---

## 📊 Dataset Summary

**Dataset Name:** Titanic Passenger Dataset  
**Source:** Kaggle (Public Dataset)  
**Number of Records:** 891  
**Number of Attributes:** 12 (reduced after cleaning)

### Key Attributes:
- PassengerId  
- Survived (Target Variable)  
- Pclass  
- Name  
- Sex  
- Age  
- SibSp  
- Parch  
- Fare  
- Embarked  

### Justification for Dataset Selection:
- Meets the requirement of at least 500 records and 8–10 attributes
- Contains both numerical and categorical variables
- Includes missing and inconsistent data suitable for cleaning
- Widely used real-world dataset for data mining and predictive modeling

---

## 🧹 Data Cleaning and Preparation

The following data cleaning steps were performed:

### 1. Handling Missing Values
- **Age:** Missing values were imputed using the median to preserve the distribution.
- **Embarked:** Missing values were filled using the mode.
- **Cabin:** Removed due to excessive missing values.

### 2. Removing Duplicates
- The dataset was checked for duplicate rows.
- Any detected duplicates were removed to avoid skewed analysis.

### 3. Handling Noisy and Inconsistent Data
- The dataset was inspected for invalid values such as negative ages.
- No significant noisy data remained after cleaning.

---

## 📈 Exploratory Data Analysis (EDA)

EDA was conducted using Matplotlib and Seaborn to explore distributions, relationships, and patterns.

### Visualizations Included:
- Age distribution histogram
- Survival count comparison
- Survival rate by gender
- Correlation heatmap for numerical attributes

### Key Insights:
- Female passengers had a higher survival rate than males.
- Passenger class strongly influenced survival outcomes.
- Age showed a moderate relationship with survival.
- Fare and passenger class were correlated, indicating socio-economic influence.

---

## 🔍 Insights for Future Modeling

Based on EDA findings:
- **Sex**, **Age**, and **Pclass** are strong predictors of survival.
- These features will be prioritized in regression and classification models.
- Feature engineering can further improve predictive performance.

---

## ⚠️ Challenges Encountered

### Challenge 1: Missing Data
- Several attributes contained missing values.
- **Solution:** Appropriate imputation and column removal techniques were applied.

### Challenge 2: Mixed Data Types
- The dataset included both categorical and numerical features.
- **Solution:** Careful inspection ensured compatibility with future modeling.

### Challenge 3: Feature Retention Decisions
- Determining which attributes to retain required balancing data quality and relevance.
- **Solution:** Data-driven decisions based on missing value percentages and analytical importance.

---

## 📁 Repository Contents

- `MSCS_634_ProjectDeliverable_1.ipynb` – Jupyter Notebook containing code, visualizations, and explanations  
- `README.md` – Project summary, data preparation steps, insights, and challenges  

---

## ✅ Conclusion

This deliverable successfully prepared the dataset for advanced data mining by performing comprehensive data cleaning and exploratory analysis. The insights gained form a strong foundation for regression modeling, classification, and clustering tasks in subsequent deliverables.

---
