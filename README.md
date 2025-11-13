# Brussels Air Quality Monitoring – Impact Assessment

> Internship-ready case study by **Clara Gracieux** showcasing advanced data-wrangling, statistical testing, and stakeholder storytelling skills.

## Executive Snapshot
_WHO (World Health Organization) recommends a daily mean PM2.5 limit of 15 µg/m³; exceeding it triggers health-risk mitigation._
| Question | Outcome |
| --- | --- |
| Weekly PM2.5 behavior | Peaks early in the workweek (Tue–Wed) with consistent weekend elevations. |
| Compliance vs. WHO guidelines | 84% of spring days exceed 15 µg/m³; Binomial test p-value ≈ 0 confirms chronic exceedance. |
| Incident attribution | Fire on 27 Aug drives a +22 µg/m³ hourly increase; z-test p-value 2.5e-12 establishes causal impact. |

## Context & Role
- **Client scenario** – Brussels environmental agency needs to substantiate alerts and quantify the effect of a critical incident.
- **Mission objective** – Deliver rapid, defensible insights that can back policy decisions (traffic restrictions, public advisories) and guide remediation budgets.
- **My contribution** – Solo analyst handling ingestion, feature engineering, exploratory analytics, inferential statistics, and executive-ready reporting.

## Data & Technology
- `treated_AQI_data_station_2.xlsx`: 3,760 hourly records (Feb–Sep 2025) with PM2.5, temperature, wind, timestamp.
- Derived artifacts inside the notebook: spring (Mar–May) aggregate, weekday summaries, incident vs. baseline comparison set.
- **Stack**: Python 3.11 · pandas · NumPy · Matplotlib · SciPy · Jupyter Notebook.

## Analytical Approach
1. **Data engineering** – Clean timestamps, build daily aggregates, enrich with weekday labels, and isolate business-critical windows.
2. **Exploratory analytics** – Visualize trends, compute descriptive statistics, and flag anomalies to guide stakeholders toward high-risk days.
3. **Hypothesis testing** –
   - One-sided Binomial test validates the “>35%” exceedance claim.
   - One-sided z-test isolates the fire’s incremental impact vs. the previous week.
4. **Insight packaging** – Each section of the notebook links methods to operational takeaways, mirroring how I would brief non-technical sponsors.

## Key Findings & Actions
- **Spring exceedances**: 68/81 days breach WHO thresholds → justification for continued heightened alerts.
- **Operational cadence**: Tuesday/Wednesday show the most severe averages → prioritize enforcement and communication during early-week rush hours.
- **Incident response**: +22 µg/m³ hourly delta linked to the fire → evidence to trigger emergency protocols and after-action reviews.

## Repository Layout
- `HW1_group02.ipynb` – Main narrative notebook (business framing, code, visuals, decisions).
- `treated_AQI_data_station_2.xlsx` – Raw monitoring feed.

## Extension Ideas
- Blend in meteorological or traffic datasets to pinpoint root causes of spikes.
- Operationalize alerts via Streamlit/Power BI dashboards or automated email digests.
- Generalize the notebook into a playbook for rapid-response environmental investigations.

Interested in collaborating or discussing these techniques? I’m happy to walk you through the project in more detail.
