# 📉 Telecom Customer Churn Analysis & Prediction

### 🚀 Project Overview
Customer retention is one of the most critical growth metrics for subscription-based businesses. This project builds an end-to-end machine learning pipeline to predict customer churn with **91.60% accuracy**. By identifying high-risk subscribers before they cancel, this model provides actionable, data-driven business recommendations to maximize revenue retention.

---

## 📊 Key Findings & Business Insights

### 1. The Day-Charge Billing Threshold (`Total day charge`)
* **Observation:** The machine learning model identified daytime charges as the number one predictor driving customer drop-offs.
* **Business Insight:** High-volume daytime users are experiencing "bill shock." They face an expensive, volatile pricing structure that penalizes heavy usage, driving them straight to competitors.
* **Recommendation:** Introduce a capped "Unlimited Corporate/Daytime" tier to convert high-risk, volatile spenders into predictable, loyal monthly subscribers.

### 2. The Customer Service Fatigue Point (`Customer service calls`)
* **Observation:** Exploratory Data Analysis (EDA) shows that the probability of customer churn spikes aggressively after a subscriber calls support more than 3 times.
* **Business Insight:** A 4th customer service call represents a critical frustration threshold where standard customer support loops fail to resolve core issues.
* **Recommendation:** Implement an automated CRM trigger. Once an account logs its 3rd support call, automatically escalate the ticket away from general queues directly to a specialized **Customer Retention Team** equipped to offer credits or tailored contract solutions.

### 3. The International Plan Optimization Flaw (`International plan`)
* **Observation:** Subscribers with an international plan activated are leaving the service at a highly disproportionate rate.
* **Business Insight:** The add-on international feature is failing to deliver long-term value, likely burdened by hidden overage fees or poor connectivity packages.
* **Recommendation:** Revamp the international bundle structure by partnering with global networks to offer flatter, simpler premium pricing packages instead of unpredictable pay-per-minute structures.

---

## 🛠️ Tech Stack & Libraries Used
* **Language:** Python
* **Environment:** Google Colab / Jupyter Notebook
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Decision Tree Classifier, Train-Test Split, Metrics)

---

## ⚙️ Workflow Architecture

### 1. Data Processing & Cleaning
* Checked for missing values and structural data anomalies.
* Converted object variables (`International plan`, `Voice mail plan`) into numeric binary codes (`1` and `0`).
* Isolated the target classification vector (`Churn`).

### 2. Machine Learning Modeling
* Leveraged an 80/20 train-test split using the predefined datasets.
* Trained a **Decision Tree Classifier** restricted to `max_depth=4` to optimize structural clarity and prevent model overfitting.
* Achieved a final test **Accuracy Score of 91.60%**.
