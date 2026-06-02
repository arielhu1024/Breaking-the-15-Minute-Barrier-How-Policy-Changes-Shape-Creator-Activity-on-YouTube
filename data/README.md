# Data

## Overview

The raw dataset used in this project is not publicly distributed due to storage limitations and YouTube API data usage restrictions.

Data were collected directly through the YouTube Data API v3 and processed into creator-level and creator-month panel datasets for analysis.

---

## Data Collection

### Source

- YouTube Data API v3

### Collection Period

- January 2010 – December 2011

### Raw Data

The original collection contains more than:

- 1.27 million video records

Each observation includes:

- Video ID
- Upload timestamp
- Video duration
- View count
- Like count
- Comment count
- Creator information

---

## Final Analytical Sample

### General Creators

| Metric | Value |
|----------|----------|
| Creators | 494 |
| Videos | 82,664 |
| Creator-Month Observations | 11,856 |

### Professional Creators

| Metric | Value |
|----------|----------|
| Top Channels | 30 |
| Creator-Month Observations | 351 |

---

## Data Processing

The raw API responses were processed using a Kafka-PySpark pipeline.

Major processing steps include:

1. JSON parsing
2. Timestamp conversion
3. Duration conversion
4. Deduplication
5. Data cleaning
6. Standardization
7. Creator-month aggregation

---

## Constructed Variables

### Content Production

- Monthly Video Count
- Long-Form Video Indicator

### Engagement Measures

- Monthly Views
- Monthly Likes
- Monthly Comments

### Policy Variables

- Post Policy Indicator
- Treatment Group Indicator
- DID Interaction Term

### Event Study Variables

- Relative Event Time
- Lead Indicators
- Lag Indicators

---

## Data Availability

The complete raw dataset is not included in this repository.

The repository provides:

- Data construction pipeline
- Feature engineering code
- Statistical outputs
- Summary results

Researchers interested in replication may reproduce the dataset using the code provided in the `notebooks/` directory and access to the YouTube Data API.

---

## Folder Structure

```text
data/
└── README.md
```

No raw data files are distributed with this repository.
