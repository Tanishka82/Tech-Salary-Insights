# 💼 Glassdoor Tech Salary Prediction (2017–2018)

This project explores tech job postings from Glassdoor with the goal of predicting salary estimates using Machine Learning. It involves in-depth data cleaning, feature engineering, EDA, and multiple regression models — concluding with a Random Forest model optimized for performance and interpretability.

---

## 📌 Project Objectives

- Analyze salary patterns across job roles, locations, company types, and required skills.
- Build a predictive model for salary estimation based on job attributes.
- Apply model evaluation and tuning techniques for best performance.
- Communicate business impact and feature importance clearly.

---

## 📊 Dataset Overview

- **Source**: Glassdoor.com (Web-scraped)
- **Records**: ~1,000 US tech job postings
- **Timeframe**: 2017–2018
- **Features**: Job Title, Salary Estimate, Location, Rating, Revenue, Skills (Python, AWS, etc.), and more.

---

## 🧹 Workflow Summary

### 1. 🧼 Data Cleaning & Preprocessing
- Removed rows with invalid or missing salary data.
- Parsed and engineered `min_salary`, `max_salary`, `avg_salary_log`, `job_simplified`, `seniority`, etc.
- Created dummy variables for categorical features.

### 2. 📈 Exploratory Data Analysis
- Salary distribution by title, seniority, location, skills, and company attributes.
- Bivariate & multivariate relationships with correlation heatmaps and bar charts.

### 3. 🤖 Model Building
Tested and evaluated:
- `Linear Regression`
- `Support Vector Regression (SVR)`
- ✅ `Random Forest Regressor` (Final Model)

### 4. 🔍 Model Evaluation
- Used metrics: `MAE`, `MSE`, `R² Score`
- Applied cross-validation and hyperparameter tuning (GridSearchCV)
- Final model R² Score: **0.9724**

### 5. 🧠 Model Explainability
- Used `feature_importances_` from Random Forest to identify key salary drivers.
- `avg_salary_log`, `Rating`, and `Company Age` emerged as top predictors.

---

## 💼 Business Impact

- Helps job seekers identify high-paying roles and essential skillsets.
- Empowers employers and recruiters to benchmark salaries more accurately.
- Promotes data-driven and fair compensation decision-making.

---

## 🧪 Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter/Colab

---

## 📁 Repository Structure

```
📦 Tech-Salary-Insights
 ┣ 📄 Glassdoor_ML_Project.ipynb
 ┣ 📄 README.md
 ┣ 📄 best_rf_model.joblib
 ┣ 📄 requirements.txt
```

---

## ▶️ Run on Colab

[![Open In Colab](https://colab.research.google.com/drive/1nnrRliX-nwuG6F4ty7sbcjEYUsf1rTyf?usp=sharing)

---

## 🙌 Author

👩‍💻 Tanishka Patil  
📬 [LinkedIn](www.linkedin.com/in/tanishkapatil08) | [GitHub](https://github.com/Tanishka82)

---

## 📌 License

This project is for educational and academic purposes only. Data belongs to respective owners (Glassdoor.com).
