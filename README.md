# 🚀 Streak Feature Impact Analysis (PlaySimple Games Case Study)

## 📌 Overview

This project analyzes whether **streak-based gameplay mechanics** improve user engagement and satisfaction in mobile games published by PlaySimple Games.

Using real user reviews from the Google Play Store, the analysis simulates how a **Business Analyst** would evaluate product features and generate actionable insights.

---

## 🎯 Problem Statement

PlaySimple games rely heavily on **daily engagement mechanics** like streaks.

The goal of this analysis is to answer:

* Do streak features improve user satisfaction?
* Are streak users more engaged than others?
* How does sentiment vary across users and over time?

---

## 📊 Dataset

* Source: Google Play Store Reviews
* App: TripCross (PlaySimple Games)
* Reviews Collected: **2000+**
* Fields Used:

  * Review text (`content`)
  * Rating (`score`)
  * Date (`at`)
  * Version info

---

## 🧠 Methodology

### 1. Data Collection

* Scraped reviews using `google-play-scraper`
* Converted raw JSON into structured DataFrame

---

### 2. Data Cleaning

* Removed null values
* Standardized text
* Converted date to monthly periods

---

### 3. Feature Engineering

Created a behavioral segment:

* **Streak Users** → Users mentioning keywords like:

  * streak, daily, reward, login, habit, bonus
* **Non-Streak Users**

---

### 4. Sentiment Analysis

* Used **VADER Sentiment Analyzer**
* Generated sentiment scores between **-1 to +1**

---

### 5. KPI Computation

Key metrics calculated:

* Average sentiment score
* Streak vs Non-streak comparison
* Absolute sentiment improvement (Δ)
* Rating distribution
* Sentiment trend over time

---

## 📈 Key Findings

### 🔥 1. Streak Features Drive Higher Engagement

* Streak Users Sentiment: **0.26**
* Non-Streak Users Sentiment: **0.03**

👉 **Absolute Improvement: +0.23**

> Users engaging with streak mechanics are significantly more satisfied.

---

### ⭐ 2. Better Ratings from Streak Users

* Streak users consistently provide **higher ratings**
* Indicates stronger engagement and retention

---

### ⚠️ 3. Low Feature Adoption

* Only **~8.6% of users mention streak-related behavior**

👉 Suggests:

* Low awareness OR
* Implicit usage without recognition

---

### 📊 4. Sentiment Trends Over Time

* Significant dip in **Sept–Nov**
* Recovery and improvement after **Jan 2026**

👉 Possible impact of product updates or fixes

---

## ⚠️ Limitations

* Keyword-based detection may miss implicit streak usage
* Potential **selection bias**:

  * Engaged users more likely to mention streaks
* Sentiment analysis may not capture sarcasm or nuance

---

## 🚀 Business Recommendations

### 1. Increase Feature Visibility

* Highlight streaks during onboarding
* Add UI nudges and progress indicators

---

### 2. Improve Incentive Design

* Better rewards for streak continuation
* Introduce milestone bonuses

---

### 3. Target Non-Streak Users

* Push notifications for daily engagement
* Personalized reminders

---

### 4. Monitor Sentiment Trends

* Track sentiment after feature releases
* Quickly respond to dips in user satisfaction

---

## 📊 Visualizations

### Sentiment Comparison

* Streak vs Non-Streak users

### Rating Distribution

* Shows skew towards lower ratings → improvement opportunity

### Sentiment Trend Over Time

* Identifies product performance across months

*(Graphs available in `/images` folder or notebook)*

---

## 🧠 Key Takeaway

> Streak mechanics are strongly associated with higher user satisfaction, but low adoption suggests a major opportunity to improve visibility and drive engagement at scale.

---

## 🛠 Tech Stack

* Python (Pandas, NumPy)
* VADER Sentiment Analysis
* Matplotlib
* Google Play Scraper

---

## 📂 Project Structure

```
streak-analysis-playsimple/
│
├── data/
│   └── raw_reviews.csv
│
├── notebook/
│   └── streak_analysis.ipynb
│
├── images/
│   ├── sentiment_comparison.png
│   ├── rating_distribution.png
│   ├── sentiment_trend.png
│
├── README.md
```

---

## 💼 Why This Project Matters

This project simulates real-world work done by a **Business Analyst at PlaySimple Games**, including:

* Product feature evaluation
* User segmentation
* KPI-driven analysis
* Actionable business insights

---

## 🔗 Future Improvements

* Topic modeling (ads, bugs, gameplay issues)
* Cohort analysis
* Retention prediction
* Advanced NLP for feature detection

---

## 🙌 Author

Built as part of preparation for **Associate Business Analyst role at PlaySimple Games**

---
