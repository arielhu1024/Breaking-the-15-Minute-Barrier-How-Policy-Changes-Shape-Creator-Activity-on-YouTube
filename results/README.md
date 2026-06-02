# Results

This folder contains the main empirical results reported in the project.

The analyses evaluate how YouTube's removal of the 15-minute upload limit in December 2010 affected creator behavior and engagement outcomes.

---

## Files

### descriptive_statistics.csv

Summary statistics for the final creator-month panel datasets.

Variables include:

- Monthly video production
- Views
- Likes
- Comments
- Long-form content indicators
- Treatment group indicators

---

### did_results_general_creators.csv

Difference-in-Differences (DID) estimates for the general creator sample.

Sample:

- 494 creators
- 82,664 videos
- 11,856 creator-month observations

Models:

- OLS Fixed Effects
- Poisson Regression
- Negative Binomial Regression

Outcomes:

- Monthly Video Count
- Likes
- Comments
- Views

Main finding:

> General creators experienced significant declines in content production and engagement following the policy change.

---

### did_results_professional_creators.csv

Difference-in-Differences (DID) estimates for the professional creator sample.

Sample:

- Top 30 YouTube channels in 2010
- 351 creator-month observations

Model:

- Creator Fixed Effects
- Month Fixed Effects

Outcomes:

- Monthly Video Count
- Likes
- Comments

Main finding:

> Professional creators increased posting activity and engagement after the removal of the 15-minute upload limit.

---

### event_study_general_creators.csv

Event-study estimates for the general creator sample.

Reference period:

- Event Time = -1

Columns:

| Variable | Description |
|----------|-------------|
| Event_Time | Months relative to policy implementation |
| Coefficient | Estimated treatment effect |
| Std_Error | Standard error |
| CI_Lower | Lower bound of 95% confidence interval |
| CI_Upper | Upper bound of 95% confidence interval |
| Significance | Statistical significance indicator |

Purpose:

- Test parallel trends assumption
- Examine dynamic treatment effects before and after the policy change

---

### event_study_professional_creators.csv

Event-study estimates for the professional creator sample.

Reference period:

- Event Time = -1

Columns:

| Variable | Description |
|----------|-------------|
| Event_Time | Months relative to policy implementation |
| Coefficient | Estimated treatment effect |
| Std_Error | Standard error |
| CI_Lower | Lower bound of 95% confidence interval |
| CI_Upper | Upper bound of 95% confidence interval |

Purpose:

- Validate DID results
- Evaluate pre-treatment trends
- Examine the timing of policy effects

---

## Key Findings

| Creator Type | Result |
|-------------|---------|
| General Creators | Reduced content production and engagement |
| Professional Creators | Increased posting activity and engagement |

The comparison reveals substantial heterogeneity in creator responses. While the policy appears to have benefited professional creators with greater production capabilities, general creators experienced declines in both activity and audience engagement.

This divergence highlights how platform policy changes can generate unequal outcomes across creator groups.
