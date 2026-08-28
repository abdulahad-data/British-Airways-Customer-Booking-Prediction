# British Airways: Predictive Modeling & Customer Sentiment Analysis

## 📌 Objective
This repository contains a data science simulation executed for British Airways via Forage. The objective was to scrape and analyze customer feedback, and subsequently build a predictive machine learning model to forecast customer booking behavior, enabling targeted marketing resource allocation.

## ⚙️ Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (Random Forest Classifier, Label Encoding)
* **Visualization:** Matplotlib, Seaborn

## 🤖 Predictive Modeling (Random Forest)
* Engineered features by converting categorical text data (`sales_channel`, `route`, `trip_type`) into numeric variables.
* Trained a Random Forest Classifier to predict the `booking_complete` target variable.
* Extracted the `.feature_importances_` array to identify the primary drivers of customer conversion.

## 💡 Key Business Insights
Based on the Random Forest feature importance extraction, the top three variables driving booking completions are:
1. **Purchase Leads**
2. **Routes**
3. **Flight Houts**

**Recommendation:** Marketing and pricing teams should aggressively target promotions based on **Purchase Leads**, as it mathematically holds the highest predictive weight for finalized revenue.
