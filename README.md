# Mobile App User Retention Analysis

> Understanding why users leave and what the data says about keeping them.

---

## The Business Problem

For any mobile app, acquiring users is expensive. Losing them is more expensive. This project investigates user retention patterns to answer the question product teams lose sleep over:

**Why do users stop coming and at what point does it happen?**

Understanding this helps app businesses prioritize the right fixes: making improvements, feature changes, or re-engagement campaigns instead of guessing.

---

## Key Questions Investigated

- What does the retention curve look like over the first 30 days?
- Are there specific drop off points where the app loses a large number of users?
- Which user segments retain better than others?
- What behavioral signals predict churn before it happens?

---

## Key Findings

See [Insights.md](./Insights.md) for the full breakdown. Highlights include:

- **Significant early drop-off** The steepest user loss happens within the first few days, pointing to an onboarding or first-session experience problem
- **Returning users show stronger long-term retention** Users who return at least once in their first week have measurably higher 30-day retention
- **Retention varies meaningfully by user segment** Not all users behave the same; segment-level analysis reveals which cohorts to prioritize

**So what does this mean?** A product team acting on these findings would focus engineering effort on the first-session experience, add a Day 1-3 re-engagement trigger, and build a retention dashboard to track improvements over time.

---

## Dataset

| Column | Description |
|---|---|
| User ID | Unique identifier per user |
| Install Date | When the user first downloaded the app |
| Session Data | Activity records per user |
| Retention Flags | Whether a user returned on Day 1, 7, 30 |
| Segment | User group or cohort classification |

---

## Methodology

1. **Cohort Analysis** Grouped users by install date to measure retention across time windows
2. **Drop-off Identification** Pinpointed exact days where churn accelerates
3. **Segmentation** Compared retention rates across user groups to find patterns
4. **Visualization** Built charts to communicate findings clearly to both technical and non technical stakeholders

---

## Tech Stack

- Python
- Pandas
- Matplotlib

---

## Visualizations

Charts are available in the [Visualizations](./Visualizations) folder, including:
- Retention curve (Day 1 - Day 30)
- Cohort heatmap
- Segment comparison charts

---

## Project Structure

- Mobile-App-User-Retention/
    - analysis/               # Python analysis scripts
    - Visualizations/         # Output charts
    - Mobile app data.csv     # Dataset
    - Insights.md             # Plain-English findings and recommendations
    - README.md

---

## What's Next?

- [ ] Predictive churn model (flag "at-risk" users before they leave)
- [ ] A/B test simulation measuring impact of onboarding changes on Day 7 retention
- [ ] Interactive retention dashboard using Plotly or Power BI
- [ ] Push notification timing analysis

---
