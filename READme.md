# **Decoding Used Car Prices: Insights for Dealership Success**

## **Overview**

This project explores a dataset of used cars to uncover factors influencing their pricing. By leveraging historical data and predictive modeling, the analysis provides actionable insights to help dealerships optimize inventory and pricing strategies.

The dataset, sourced from Kaggle, includes 426,000 records with attributes such as car make, model, year, mileage, fuel type, and other features influencing value.

---

## **Business Understanding**

Dealerships need to maximize revenue by efficiently pricing and selling vehicles. This project identifies the most critical factors influencing car prices, helping dealerships:

* Stock high-value vehicles.  
* Optimize pricing strategies based on key attributes.  
* Minimize inventory churn.

---

## **Data Preparation**

### **Data Cleaning**

* Removed rows with missing critical values (e.g., 'price', 'year', 'odometer').  
* Filtered out unrealistic data (e.g., prices below $1,000 or above $100,000).

### **Outlier Handling**

* Visualized outliers in price and removed extreme values.

### **Feature Engineering**

* Created new features (e.g., car age).  
* Applied OneHotEncoding for categorical variables.  
* Removed low-variance features using Variance Threshold.

---

## **Exploratory Data Analysis (EDA)**

* Visualized price distributions before and after cleaning.  
* Used correlation heatmaps to explore relationships between key features.  
* Identified factors like mileage, condition, and manufacturer as strong predictors of price.

---

## **Modeling Approach**

### **Models**

1. **Linear Regression:** Baseline model.  
2. **Lasso Regression:** Handles multicollinearity.  
3. **Random Forest Regression:** Captures non-linear relationships.

### **Evaluation**

* Used 5-fold cross-validation with Mean Squared Error (MSE) and R² metrics.  
* Tuned hyperparameters for Lasso and Random Forest using GridSearchCV.

---

## **Key Findings**

* **Age:** Newer cars command higher prices.  
* **Mileage:** Lower odometer readings significantly boost value.  
* **Manufacturer:** Toyota and Honda models have higher average prices.  
* **Condition:** "Excellent" cars are valued up to 40% higher than "Fair" cars.  
* **Fuel Type:** Hybrid and electric vehicles are priced higher than gasoline-powered cars.

---

## 

## 

## **Recommendations**

### **Stock Smarter**

* Focus on cars under 50,000 miles.  
* Prioritize manufacturers like Toyota and Honda for consistent resale value.

### **Price Strategically**

* Use predictive models (e.g., Random Forest) to set competitive prices.  
* Apply steeper discounts for cars over 10 years old.

### **Understand Buyers**

* Highlight fuel efficiency and 4-wheel drive features in listings.

---

## **Next Steps**

1. **Enhance Data:** Add regional factors and seasonal demand trends.  
2. **Explore Advanced Models:** Use Gradient Boosting or XGBoost for improved accuracy.  
3. **Improve Interpretability:** Apply SHAP values for feature impact analysis.

---

## **Requirements**

### **Python Libraries**

* pandas  
* numpy  
* matplotlib  
* seaborn  
* scikit-learn  
* missingno

