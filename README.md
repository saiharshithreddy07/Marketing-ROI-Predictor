# 📈 Marketing Budget ROI Predictor

## 📌 Overview
This project solves a classic business problem: **"Where should we spend our marketing budget to get the highest sales?"**
Using historical ad spend data, I built a Linear Regression model to predict sales revenue based on TV, Radio, and Newspaper investments.

## 🧠 Key Strategy: Feature Engineering
Initial modeling provided ~90% accuracy. However, I hypothesized that marketing channels have a **"Synergy Effect"** (TV + Radio working together).
* **Action:** I created an interaction term (`TV * Radio`) and removed the noisy `Newspaper` variable.
* **Result:** Model accuracy jumped to **97.6%**.

## 🛠️ Technical Details
* **Algorithm:** Multiple Linear Regression (OLS)
* **Optimization:** Interaction Terms & Feature Selection
* **Tech Stack:** Python, Scikit-Learn, Statsmodels, Seaborn

## 📊 Business Insights
1.  **TV is King:** The primary driver of volume.
2.  **Radio is Efficient:** High return on investment per dollar.
3.  **Drop Newspaper:** The data showed near-zero correlation with sales, suggesting budget should be reallocated.

## 🚀 How to Run
1.  Open the `Marketing_Budget_ROI_Predictor.ipynb` file.
2.  Run the "Scenario Testing" cells to input your own budget numbers and see the predicted sales.
