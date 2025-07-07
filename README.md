
# 🚌 Red Bus Hackathon – Bus Demand Prediction

## 📌 Problem Statement

The objective of this hackathon was to **predict bus ticket demand 15 days in advance** for different routes and dates. This helps optimize seat allocation and dynamic pricing for maximum efficiency and revenue.

---

## 🗂️ Dataset Overview

The dataset provided included:

* **Train.csv** and **Test.csv**: Contain route-wise data for demand prediction.
* **Transactions.csv**: Contains detailed ticket booking transactions from **March 2023 to February 2025**.

---

## 🧪 Data Preprocessing

1. **Date-Based Splitting**:

   * Split the `transactions.csv` file into training and testing sets based on the date of the journey to simulate real-time forecasting.
2. **Exploratory Data Analysis (EDA)**:

   * Analyzed booking patterns across:

     * Days of the week (higher on **weekends**).
     * Time to journey (majority of tickets booked **within 15 days** of travel).
     * Regions and routes (some showed consistently **high demand**).
     * Holidays and special events (noticed a **spike in bookings**).

---

## 🛠️ Feature Engineering

* **Tier Combo**: Combined tiers to encode route-specific pricing and class patterns.
* **Final Seat Availability**: Adjusted seat counts for holidays and weekends.

---

## 🤖 Modeling Approaches

Used the following models for demand prediction:

* **TabularNet (AutoGluon)**

  * Deep learning-based tabular data model.
  * Captured non-linear interactions and complex patterns.

* **Random Forest Regressor**

  * Performed well with engineered features and provided strong baseline performance.

* **Autoencoders (for anomaly detection & feature compression)**

  * Used as a feature learning and dimensionality reduction technique.

---

## ✅ Results

* **TabularNet** and **Random Forest** outperformed other approaches with strong generalization on unseen data.
* Successfully captured seasonality, demand surges, and route-specific behaviors.

---

## 📌 Key Learnings

* Demand forecasting requires a deep understanding of booking behavior patterns.
* Time proximity to journey and holidays are critical indicators.
* Ensemble and automated modeling frameworks like AutoGluon can significantly accelerate model development and tuning.


