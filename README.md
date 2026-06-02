<div align="center">

# 🎬 Breaking the 15-Minute Barrier

### How Policy Changes Shape Creator Activity on YouTube

Research Project • Causal Inference • Data Engineering • Creator Economy

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Kafka-000000?style=for-the-badge&logo=apache-kafka"/>
<img src="https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apache-spark"/>
<img src="https://img.shields.io/badge/SQL-336791?style=for-the-badge"/>

</div>

---

## 🎯 Research Question

How do platform policy changes affect creator behavior?

In December 2010, YouTube removed its long-standing 15-minute upload limit for verified users. While the policy was intended to encourage richer content creation, little is known about how creators with different resources and capabilities adapt to such platform changes.

This project investigates whether the policy generated different behavioral responses among **general creators** and **professional creators**, and explores how platform design can reshape participation within digital content ecosystems.

---

## 📊 Project Snapshot

| Metric | Value |
|----------|----------|
| Videos Collected | 1.27M+ |
| Creators | 494 |
| Final Videos | 82,664 |
| Creator-Month Observations | 11,856 |
| Study Period | Jan 2010 – Dec 2011 |
| Data Source | YouTube Data API |

---

## 🔄 Research Pipeline

```text
YouTube API
      ↓
Kafka Data Collection
      ↓
PySpark ETL Pipeline
      ↓
Creator-Month Panel Dataset
      ↓
Feature Engineering
      ↓
Difference-in-Differences
Fixed Effects Models
Poisson / Negative Binomial
      ↓
Behavioral Insights
```

---

## 👥 Creator Groups

A key contribution of this project is distinguishing between two creator populations.

### General Creators

- Random sample of active YouTube creators
- Limited production resources
- Primarily individual content producers
- Represent the broader creator ecosystem

### Professional Creators

- Top-performing YouTube channels during the study period
- Greater production capacity and audience reach
- Higher ability to invest in long-form content
- Represent resource-rich creators

This distinction allows us to examine whether platform policy changes create unequal outcomes across creator groups.

---

## 🧠 Methodology

### Causal Inference

- Difference-in-Differences (DID)
- Event Study Analysis

### Panel Data Models

- Fixed Effects Models
- Creator Fixed Effects
- Month Fixed Effects

### Count Data Models

- Poisson Regression
- Negative Binomial Regression

---

## 📈 Key Findings

### General Creators

📉 Monthly uploads decreased significantly after the policy change.

📉 Likes and comments declined substantially.

📉 Overall creator activity became less frequent.

### Professional Creators

📈 Content production increased significantly.

📈 Professional creators were more likely to adopt long-form content.

📈 Resource-rich creators benefited more from the new policy environment.

---

## 💡 Main Insight

The removal of YouTube's upload limit did not affect all creators equally.

While the policy expanded opportunities for long-form content, creators with greater resources and production capabilities were better positioned to take advantage of the change.

These findings suggest that platform design decisions can unintentionally widen disparities between creator groups, producing heterogeneous outcomes across digital ecosystems.

---

## ⚙️ Technologies

### Data Collection

- YouTube Data API
- Kafka

### Data Engineering

- PySpark
- SQL

### Statistical Analysis

- Python
- Pandas
- Statsmodels

### Research Methods

- Difference-in-Differences
- Event Studies
- Fixed Effects Models

---

## 👨‍💻 My Contributions

✔ Designed the full data collection pipeline

✔ Collected over 1.27 million video records

✔ Built creator-month panel datasets

✔ Developed automated ETL workflows using Kafka and PySpark

✔ Conducted causal inference analyses

✔ Generated strategic insights on creator behavior and platform governance

---

## 📬 Author

**Ariel Hu**

M.S. Business Analytics  
University of Arizona

Research Interests:

- Artificial Intelligence
- Machine Learning
- Consumer Behavior
- Marketing Analytics
- Digital Platforms
