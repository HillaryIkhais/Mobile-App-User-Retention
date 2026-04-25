# Mobile App User Retention Analysis

Understanding when users drop off and what drives long-term engagement

---

## The Business Problem

Most mobile apps don’t fail because they can’t acquire users; they fail because they lose users immediately after acquisition.
This analysis identifies:
- When users stop returning
- Where the biggest drop-offs happen
- Which behaviors predict retention


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

## Core Retention Pattern
- The largest user loss happens in the first 1–3 days
- Users who survive the first week are far more likely to become long term active users
- Retention is not uniform, that is, user behavior clusters into distinct patterns

## Business Interpretation
- Retention is not a long-term problem — it is an early lifecycle problem.
This means:
- Fixing onboarding has higher ROI than adding new features
- Early engagement determines lifetime value
- Small improvements in Day 1–7 retention compound significantly


## What a product team would do with this
Based on these findings, a team would:
- Improve onboarding experience to reduce Day 1–3 drop-off
- Trigger re-engagement actions for users inactive after first session
- Prioritize product improvements for high-retention user segments
- Build retention tracking dashboards for early behavior monitoring

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

## Tools Used
- Python (Pandas, Matplotlib)

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

## Business Value
This analysis helps:
- Reduce early user drop-off
- Improve onboarding effectiveness
- Identify high value user segments
- Increase long-term user retention

---
