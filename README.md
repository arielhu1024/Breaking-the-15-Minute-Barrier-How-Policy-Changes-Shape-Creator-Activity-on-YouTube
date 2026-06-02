# Breaking the 15 Minute Barrier: How Policy Changes Shape Creator Activity on YouTube

## 📖 Project Summary

This project investigates how YouTube’s removal of the 15-minute upload limit affected creator behavior.

Using large-scale behavioral data collected through the YouTube Data API, Kafka, and PySpark, I constructed a creator-month panel dataset and applied causal inference methods to estimate the impact of platform policy changes on content production and engagement outcomes.

---

## 📊 Project Snapshot

| Item | Value |
|--------|--------|
| Videos Collected | 1.27M+ |
| Creators | 494 |
| Final Videos | 82,664 |
| Panel Observations | 11,856 |
| Time Period | Jan 2010 – Dec 2011 |
| Data Sources | YouTube Data API |

---

## 🔄 Data Pipeline

```mermaid
flowchart LR

A[YouTube API]
--> B[Kafka]

B --> C[PySpark ETL]

C --> D[Creator-Month Panel]

D --> E[DID Models]

D --> F[Fixed Effects]

D --> G[Poisson/NB Models]
```

---

## 🧠 Methodology

### Causal Inference

- Difference-in-Differences (DID)
- Event Study

### Panel Data Analysis

- Fixed Effects Models

### Count Data Models

- Poisson Regression
- Negative Binomial Regression

---

## 📈 Key Findings

- General creators reduced posting frequency after the policy change.
- Professional creators increased posting frequency.
- Platform policy changes generated heterogeneous impacts across creator groups.

---

## ⚙️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apache-spark&logoColor=white)

![Kafka](https://img.shields.io/badge/Kafka-000000?style=for-the-badge&logo=apache-kafka)

![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge)
