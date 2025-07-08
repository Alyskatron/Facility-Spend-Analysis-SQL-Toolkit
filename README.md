# Facility Spend Analysis SQL Toolkit

This repository contains a collection of SQL queries designed to analyze purchasing and spend behavior across facilities over time. These patterns are useful for trend analysis, forecasting readiness, cohort analysis, and identifying outliers.

---

## 📊 Features

- **Rolling Averages**: 3-month trailing average per facility
- **Year-over-Year Growth**: Annual spend and percentage growth
- **Pivot Tables**: Monthly comparisons across multiple years
- **Cohort Analysis**: Spend progression based on facility start month
- **Cumulative Spend**: Running total per facility over time
- **Outlier Detection**: Flag anomalous spend using z-scores
- **Variance Analysis**: Identify facilities with unstable spending

---

## 📁 Files

| File Name                          | Description |
|-----------------------------------|-------------|
| `rolling_avg_3_month.sql`         | 3-month rolling average by facility |
| `yearly_spend_and_yoy_growth.sql` | Annual spend and YoY growth |
| `monthly_spend_comparison_pivot.sql` | Monthly spend by year in pivot format |
| `facility_level_cumulative_spend.sql` | Cumulative spend per facility |
| `outlier_detection_zscore.sql`    | Z-score based outlier flagging |
| `facility_cohort_analysis.sql`    | Tracks facility spend over time from cohort month |

---

## 🧠 Data Assumptions

The queries assume a base table with at least the following fields:
- `facility_name` or `facility_id`
- `purchase_date` (in DATE format)
- `purchase_total` (numeric spend amount)

---

## 🛠 How to Use

1. Replace `your_dataset.your_table` with your actual BigQuery or SQL data source.
2. Customize filters or time windows if needed.
3. Run in your preferred SQL interface (BigQuery Console, Looker, dbt, etc.).

---

## 📈 Visualization Ideas

- Heatmaps (monthly/yearly)
- Box plots (seasonal spend)
- Cohort area charts
- Time series for cumulative or rolling averages
- Scatterplots for z-score flagged anomalies

---

## 📄 License

MIT License – free to use, modify, and distribute with attribution.

---

## 👩‍💻 Contributions

Contributions are welcome! Feel free to open an issue or submit a PR for enhancements or adaptations.

---

## 📬 Contact

Created by Alyssa Ortega – feel free to reach out with questions or collaborations.

