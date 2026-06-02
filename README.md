# Breaking the 15-Minute Barrier: How Policy Changes Shape Creator Activity on YouTube

## Overview

This project examines how YouTube's removal of the 15-minute upload limit affected creator behavior. Using large-scale behavioral data collected through the YouTube Data API, Kafka, and PySpark, I constructed a creator-month panel dataset and applied causal inference methods to evaluate the impact of the policy change on content production and engagement.

The project investigates whether platform policy changes affect all creators equally, with particular attention to differences between general creators and professional creators.

---

## Research Question

The study addresses the following questions:

1. How did YouTube's removal of the 15-minute upload limit affect creator activity?

2. Did creators increase or decrease content production following the policy change?

3. Were the effects different for general creators and professional creators?

4. What do these findings imply about platform governance and creator ecosystems?

---

## Dataset

### Data Collection

Data were collected using the YouTube Data API and processed through a Kafka-PySpark pipeline.

### Sample

- 1.27 million videos collected
- 494 creators
- 82,664 videos retained for analysis
- 11,856 creator-month observations

### Study Period

January 2010 – December 2011

---

## Methodology

The analysis combines causal inference and panel data methods.

### Data Engineering

- YouTube Data API
- Kafka
- PySpark

### Statistical Models

- Difference-in-Differences (DID)
- Event Study Analysis
- Fixed Effects Models
- Poisson Regression
- Negative Binomial Regression

---

## Creator Groups

### General Creators

A random sample of active YouTube creators representing the broader creator ecosystem.

### Professional Creators

Established creators with larger audiences and greater production resources.

The comparison between these two groups allows the study to examine heterogeneous responses to platform policy changes.

---

## Key Findings

### General Creators

- Monthly content production decreased after the policy change.
- Engagement metrics such as likes and comments declined.
- Long-form content adoption was limited.

### Professional Creators

- Content production increased significantly.
- Professional creators adopted long-form content more rapidly.
- Resource-rich creators benefited more from the policy change.

### Overall Conclusion

The policy change generated heterogeneous effects across creator groups. While professional creators expanded production, many general creators reduced activity, suggesting that platform design changes may unintentionally increase disparities within creator ecosystems.

---

## Repository Structure

```text
.
├── README.md
│
├── data/
│   └── README.md
│
├── docs/
│   └── Conference Paper.pdf
│
├── figures/
│   ├── study_design.png
│   ├── event_study_general_creators_views.png
│   └── event_study_professional_creators.png
│
├── notebooks/
│   ├── 00_environment_setup.ipynb
│   ├── 01_general_creators_youtube_api_collection.ipynb
│   ├── 02_general_creators_kafka_pyspark_pipeline.ipynb
│   ├── 03_general_creators_did_event_study.ipynb
│   ├── 04_professional_creators_data_collection.ipynb
│   ├── 05_professional_creators_did_analysis.ipynb
│   ├── 99_appendix_validation_and_robustness.ipynb
│   └── README.md
│
├── results/
│   ├── did_results_general_creators.csv
│   ├── did_results_professional_creators.csv
│   ├── event_study_general_creators.csv
│   ├── event_study_professional_creators.csv
│   └── README.md
```

---

## Running the Project

### Requirements

- Python 3.10+
- Apache Kafka
- Apache Spark
- Jupyter Notebook

### Installation

```bash
pip install pandas numpy pyspark kafka-python statsmodels
```

### Running Analysis

```bash
jupyter notebook
```

Open the notebooks in the analysis directory and execute the workflow sequentially.

---

## Dependencies

Main packages used in this project:

- pandas
- numpy
- pyspark
- kafka-python
- statsmodels
- matplotlib

---
