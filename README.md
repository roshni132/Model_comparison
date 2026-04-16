# Model_comparison
# 🏠 Enhanced House Price Prediction System (AI/ML Task 2)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![scikit-learn](https://img.shields.io/badge/Library-scikit--learn-yellow)

## 📌 Project Overview
This project is part of my AI/ML internship/learning journey (Task 2). It focuses on an industry-aligned Machine Learning workflow. Going beyond basic model training, this project involves data preprocessing, feature scaling, training multiple regression models, and making a data-driven decision to select the best-performing algorithm.

## 📊 Dataset Used
* **Name:** California Housing Dataset
* **Source:** `sklearn.datasets`
* **Target Variable:** Median House Value (`HousePrice`)
* **Features:** Median Income, House Age, Average Rooms, Population, Latitude, Longitude, etc.

## ⚙️ Methodology & Workflow
1.  **Data Loading & Preparation:** Extracted the dataset into a Pandas DataFrame for easy manipulation.
2.  **Feature Scaling (Crucial Step):** Applied `StandardScaler` to ensure all features had a fair impact on the model, preventing features with larger numeric ranges from dominating.
3.  **Train-Test Split:** Divided the dataset into an 80% training set and a 20% testing set to evaluate the models on unseen data.
4.  **Model Training & Comparison:** Trained three different regression algorithms instead of relying on just one:
    * Linear Regression (Baseline)
    * Ridge Regression (L2 Regularization)
    * Decision Tree Regressor (Non-linear pattern recognition)
5.  **Evaluation:** Used Root Mean Squared Error (RMSE) and R-squared (R²) Score to objectively measure and compare performance.

## 🏆 Results & Model Selection

| Model Name               | RMSE (Root Mean Squared Error) | R² Score |
|--------------------------|--------------------------------|----------|
| Linear Regression        | 0.7455                         | 0.5757   |
| Ridge Regression         | 0.7455                         | 0.5758   |
| **Decision Tree Regressor** | **0.7242** | **0.5997** |

**Conclusion:** The **Decision Tree Regressor** was selected as the best-performing model for this specific dataset. It achieved the lowest RMSE and the highest R² score, demonstrating its ability to capture non-linear relationships (like geographic location and income boundaries) better than the standard linear models.

## 📈 Visualizations
The project includes scatter plots visualizing the **Actual vs. Predicted House Prices** along with a perfect prediction reference line to visually validate model accuracy.

## 💻 How to Run This Project
1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
