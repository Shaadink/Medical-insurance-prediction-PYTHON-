
# 🏥 Medical Insurance Price Prediction using Machine Learning



## 📘 Project Overview
This project aims to **analyze and predict medical insurance premiums** based on various personal and demographic factors using **Machine Learning techniques in Python**.  
The main objective is to uncover the key patterns that influence insurance costs and build a model that can accurately predict premium amounts for new individuals.

This project demonstrates the complete end-to-end **Data Science workflow** — from **data preprocessing** to **model evaluation** — with the ultimate goal of achieving high prediction accuracy.

---

## 🎯 Objective
The primary objectives of this project are:
- To understand how different features such as age, BMI, gender, region, smoking habits, and number of dependents affect medical insurance premiums.  
- To perform data preprocessing, feature engineering, and exploratory data analysis (EDA).  
- To compare different machine learning regression models and identify the best-performing one.  
- To interpret the insights and business implications of the results.

---

## 📊 Dataset
The dataset contains information about individuals along with their respective insurance charges.  
Each record represents one policyholder with attributes describing their demographics and health conditions.

### **Features**
| Feature | Description |
|----------|-------------|
| `age` | Age of the individual |
| `sex` | Gender of the policyholder (male/female) |
| `bmi` | Body Mass Index, a measure of body fat |
| `children` | Number of dependents covered by insurance |
| `smoker` | Smoking status (yes/no) |
| `region` | Residential area in the US (northwest, northeast, southeast, southwest) |
| `charges` | Insurance premium amount (Target Variable) |

---

## ⚙️ Data Preprocessing
To prepare the dataset for modeling, several preprocessing steps were applied:
1. **Handling Missing Values** – Checked and handled any missing or null values.  
2. **Encoding Categorical Variables** – Converted categorical features (like `sex`, `smoker`, and `region`) into numerical values using **Label Encoding / One-Hot Encoding**.  
3. **Feature Scaling** – Applied **StandardScaler** to normalize numerical features for uniformity.  
4. **Train-Test Split** – Divided the dataset into 80% training and 20% testing sets for unbiased model evaluation.

---

## 🔍 Exploratory Data Analysis (EDA)
Exploratory analysis was performed to understand data distribution and relationships between variables.  

### **Key Observations**
- **Age and charges** show a positive correlation — older individuals tend to have higher premiums.  
- **Smokers** pay significantly higher charges compared to non-smokers.  
- **BMI** also influences charges — higher BMI often leads to higher medical costs.  
- The number of **children** has a minor impact on premium prices.  
- **Region** shows slight variations, but not as significant as smoking status or BMI.

**Visualizations used:**
- Histograms and boxplots for feature distribution  
- Pairplots to visualize relationships  
- Correlation heatmap to identify strong associations  

---

## 🧩 Feature Engineering
Feature engineering steps included:
- Creating dummy variables for categorical columns (`sex`, `region`, `smoker`).  
- Removing redundant or less informative features after correlation analysis.  
- Ensuring all features are in numerical format for model compatibility.

These steps improved the model interpretability and accuracy.

---

## 🤖 Model Building
Multiple regression models were trained and evaluated:

1. **Linear Regression**  
2. **Decision Tree Regressor**  
3. **Random Forest Regressor**  
4. **Gradient Boosting Regressor**  
5. **XGBoost Regressor**

Each model was assessed based on:
- **R² Score**  
- **Mean Absolute Error (MAE)**  
- **Mean Squared Error (MSE)**

---

## 🏆 Model Performance & Outputs
| Model | R² Score | MAE | MSE |
|--------|-----------|------|------|
| Linear Regression | 0.75 | Moderate | High |
| Decision Tree | 0.85 | Low | Medium |
| Random Forest | 0.89 | Lower | Lower |
| Gradient Boosting | 0.91 | Low | Lower |
| **XGBoost** | **0.94** | **Lowest** | **Lowest** |

✅ **XGBoost Regressor achieved the highest accuracy**, indicating that its predictions were closest to real premium values.  
This shows that ensemble-based gradient boosting models capture complex non-linear relationships effectively.

---

## 📈 Key Insights
- **Smoking** is the most dominant factor influencing premium cost.  
- **Age** and **BMI** are strong predictors of medical expenses.  
- The **number of children** has minimal effect on premium variation.  
- **XGBoost** outperformed all other models with the best predictive power.  
- Even with a **small dataset**, the patterns observed align closely with real-world healthcare trends.

---

## 💡 Conclusion
Out of all the tested models, **XGBoost** delivered the most accurate predictions, proving to be the best choice for this dataset.  
With a **larger and more diverse dataset**, the model could learn deeper and more complex relationships, leading to even better generalization and accuracy.

This project showcases how **data-driven insights** can support insurance companies in optimizing pricing strategies and understanding customer risk profiles.

---

## 🛠️ Tech Stack
- **Programming Language:** Python  
- **Libraries Used:** pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost  

---

## 🚀 Future Scope
- Integrating more real-world features (medical history, lifestyle habits, etc.).  
- Building a web application for real-time premium prediction.  
- Deploying the model using Flask or Streamlit for end-user interaction.

---
