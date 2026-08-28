# British Airways: Predictive Modeling & Customer Sentiment Analysis

## 📌 Objective
This repository contains a dual-phase data science simulation executed for British Airways via Forage. The objective was to scrape and analyze customer feedback, and subsequently build a predictive machine learning model to forecast customer booking behavior, enabling targeted marketing resource allocation.

## ⚙️ Tech Stack
* **Language:** Python
* **Data Extraction:** BeautifulSoup, Requests
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (Random Forest Classifier, Label Encoding)
* **Visualization:** Matplotlib, Seaborn

## 📊 Phase 1: Web Scraping & Data Cleaning
* Extracted customer reviews directly from the Skytrax website using BeautifulSoup.
* Cleaned unstructured text data using Pandas string manipulation to remove verification tags and HTML artifacts.
* Prepared the text data for baseline sentiment analysis to track brand perception.

## 🤖 Phase 2: Predictive Modeling (Random Forest)
* Engineered features by converting categorical text data (`sales_channel`, `route`, `trip_type`) into numeric variables.
* Trained a Random Forest Classifier to predict the `booking_complete` target variable.
* Extracted the `.feature_importances_` array to identify the primary drivers of customer conversion.

## 💡 Key Business Insights
Based on the Random Forest feature importance extraction, the top three variables driving booking completions are:
1. **Purchase Leads**
2. **Routes**
3. **Flight Houts**

**Recommendation:** Marketing and pricing teams should aggressively target promotions based on **Purchase Leads**, as it mathematically holds the highest predictive weight for finalized revenue.
