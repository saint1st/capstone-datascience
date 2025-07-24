# 📊 Google Advanced Data Analytics Capstone Project

**Program**: [Google Advanced Data Analytics Professional Certificate](https://www.coursera.org/professional-certificates/google-advanced-data-analytics)  
**Objective**: Analyze employee data to understand attrition, key performance drivers, and recommend retention strategies.

---

## 🧠 Project Overview

This capstone project investigates a real-world HR dataset containing employee details such as satisfaction, evaluation scores, department, salary level, and attrition status. The goal is to derive insights from employee behaviors and identify predictors of turnover using exploratory analysis and modeling techniques.

---

## 📦 Dataset Information

- **Source**: CSV file (`HR_capstone_dataset.csv`)
- **Records**: 14,999 employee entries
- **Columns**:
  - `satisfaction_level`
  - `last_evaluation`
  - `number_project`
  - `average_monthly_hours`
  - `tenure` (time spent in company)
  - `work_accident`
  - `promotion_last_5years`
  - `department`
  - `salary`
  - `left` (attrition label)

---

## 🔍 Key Steps

### 1. 🧹 Data Cleaning & Preprocessing

- Renamed columns for consistency
- Removed 300+ duplicate rows
- Checked for missing values (none found)
- Outlier analysis using boxplots

### 2. 📊 Exploratory Data Analysis (EDA)

- Analyzed attrition based on salary, satisfaction, evaluation, and tenure
- **Insights**:
  - Most leavers had low satisfaction or high workload (projects/monthly hours)
  - Higher attrition seen among low-salary employees
  - Employees who were promoted had lower attrition rates

**Visualizations included**:
- Countplots of attrition vs salary
- KDE plots of satisfaction by attrition group
- Correlation heatmaps
- Department-wise attrition distribution

### 3. ⚙️ Feature Engineering

- Converted categorical variables using one-hot encoding
- Created combined workload indicator

### 4. 🤖 Predictive Modeling

Applied machine learning models:
- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors
- Support Vector Machine (SVM)

**Metrics Evaluated**:
- Accuracy
- Confusion Matrix
- Precision, Recall, F1 Score

**Best Model**:  
✅ **Random Forest** with ~98% accuracy  
📌 Important Features: `satisfaction_level`, `tenure`, `last_evaluation`
