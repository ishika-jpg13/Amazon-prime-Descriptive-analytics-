# Amazon Prime Video User Analytics

**A Descriptive Analytics Report** | Power BI + simulated 100-user dataset (July 2026)

---

## Overview

This repository contains the report, dataset documentation and supporting files for a Business Analytics assignment. The study summarises **what the data shows** (descriptive analytics only, no forecasting) across demographics, content, viewing behaviour, devices, subscription plans and cross-variable relationships.

> **Note on data:** Real Prime Video subscriber data is proprietary. The dataset is a **simulated** sample built to reproduce the totals and splits of the source Power BI dashboard.

## Project Details

| Field | Details |
|---|---|
| Product | Amazon Prime Video (global video-streaming platform) |
| Submitted by | Ishika Shrivastava |
| Roll No. / Section | 60 / BCADS23 |
| Submitted to | Ms. Monica |
| University | Babu Banarasi Das University (BBD University), Lucknow |
| Submission date | 21 August 2026 |
| BI tool | Power BI |

## Objectives

1. Who are the users? (age and gender profile)
2. What do they watch? (genre popularity)
3. How do they rate content, and does the most-watched genre also rate highest?
4. How does daily engagement change across the month?
5. What devices do they watch on?
6. What plans do they pay for? (Basic / Standard / Premium)
7. Which titles get the most attention?
8. Which relationships appear only when variables are cross-tabulated? (gender, plan, device, rating)

## Dataset at a Glance

| Attribute | Value |
|---|---|
| Users (rows) | 100 |
| Period | 31 days, July 2026 |
| Fields | User_ID, Age, Gender, Plan, Genre, Rating, Device, Hrs |
| Total watch time | ~10,000 hours (100.0 hrs per user on average) |
| Distinct titles / genres / plans | 24 / 8 / 3 |

See `Dataset.pdf` for the full data dictionary and a 30-row sample. A CSV copy of the sample is in `prime_video_sample.csv`.

## Key Findings

| Area | Finding |
|---|---|
| Demographics | Mean/median age 26.5 (SD 5.69); 58% male, 42% female; secondary peak at age 35 (12 users) |
| Genre | Sci-Fi most watched (17 users); Thriller least (9) |
| Ratings | Overall 4.00/5; Documentary and Drama highest (4.2+); Comedy lowest (~3.6) |
| Daily trend | Peak ~610 (Day 3), low ~190 (Day 10); engagement is event-driven, not flat |
| Devices | TV 29.32%, Mobile 24.74%, Tablet 23.80%, Laptop 22.13% |
| Plans | Standard 36%, Premium 34%, Basic 30% |
| Titles | *The Boys* and *Fallout* tied at 7 viewers; long tail of niche titles |
| Cross-tabs | 43% of women are on Premium vs 28% of men; 77% of Basic users are male; Premium out-watches other plans on every device (121.0 hrs avg) |

## Repository Structure

```
Amazon-Prime-Video-User-Analytics/
|-- README.md
|-- Dataset.pdf                 # data dictionary + 30-row sample
|-- Ishika_60_DA_Report.pdf     # full 17-page descriptive report
|-- prime_video_sample.csv      # machine-readable 30-row sample
`-- dashboard.pbix              # Power BI dashboard (optional)
```

## Report Contents

| Figure | Topic |
|---|---|
| Fig. 1-2 | Age and gender distribution |
| Fig. 3-4 | Genre distribution and average rating by genre |
| Fig. 5 | Daily watch time trend |
| Fig. 6 | Device usage |
| Fig. 7 | Subscription plan distribution |
| Fig. 8 | Top watched titles |
| Fig. 9-11 | Cross-tabulations (plan x gender, rating x gender x genre, device x plan) |
| Fig. 12 | Composite Power BI dashboard (appendix) |

## Next Steps (Descriptive to Predictive)

- Churn forecasting per segment using watch-hour and rating trends
- Anomaly detection on sudden drops in watch time or title ratings
- Recommendation tuning using the popularity-vs-rating gap (Documentary / Drama)
- Cohort and retention analysis by subscription plan

## References

- Amazon Prime Video User Analytics Dashboard (Power BI, July 2026)
- Simulated Prime Video subscriber dataset (n = 100)
- McKinney, W. (2022). *Python for Data Analysis* (3rd ed.). O'Reilly Media.
- Course materials: Business Analytics - Descriptive Analytics Assignment Brief (2026)

---

*Prepared for academic purposes. Amazon and Prime Video are trademarks of their respective owners; this project is not affiliated with Amazon.*
