# Marketing Measurement & Incrementality Analysis — DACH Region

### Simulating a Measurement Implementation Expert workflow for a privacy-first advertising environment

**Dataset:** 3 years of simulated daily marketing data · 3,288 observations · 3 DACH markets  
**Methods:** Conversion Lift · Incrementality Analysis · Statistical Significance Testing · Marketing Mix Modeling · SQL Analytics · ROI Optimization

---

## Key Results

| Market | ROI | ROAS | Conversion Lift | StatSig | Budget Change |
|--------|-----|------|-----------------|---------|---------------|
| 🇨🇭 Switzerland | **1,144.3%** | 19.14x | +50.0% | Yes | +22.8% |
| 🇦🇹 Austria | 597.8% | 10.74x | +15.8% | No | -3.9% |
| 🇩🇪 Germany | 290.6% | 6.00x | -16.4% | No | -18.9% |

---

## Business Context

Privacy changes across Europe have fundamentally shifted how digital advertising
performance is measured. With user-level tracking becoming increasingly limited,
marketers can no longer rely solely on traditional attribution models to understand
whether their campaigns are driving real business impact.

This project simulates the role of a **Measurement Implementation Expert** supporting
a mid-size e-commerce company operating across the **DACH region**. The client has
been running Google Ads campaigns consistently, but leadership is questioning whether
the observed conversions are truly incremental — or whether users would have converted
anyway, with or without advertising exposure.

---

## Business Problem

Three core questions drive this analysis:

- Are Google Ads campaigns generating **incremental** conversions, or just capturing
  demand that already existed?
- Which marketing channels contribute most to business outcomes across the DACH region?
- How should budgets be allocated across **Germany, Austria and Switzerland** to
  maximize return?

---

## Why the DACH Region Is Particularly Interesting

| | 🇩🇪 Germany | 🇦🇹 Austria | 🇨🇭 Switzerland |
|---|---|---|---|
| **Ad receptiveness** | Lower | Medium | Higher |
| **Digital engagement** | Moderate | Moderate | Strong |
| **Purchasing power** | High | Medium | Very high |
| **Role in this analysis** | Scale market | Mid-tier | Efficiency leader |

Skepticism toward advertising is a shared DACH trait, but its intensity varies
significantly by country. **German consumers** are well-documented in their preference
for transparent, fact-based communication and their resistance to persuasion-driven ads —
a pattern that shows up directly in lower CTRs, higher CPAs and, in this analysis,
a **negative Conversion Lift**. **Switzerland**, despite sharing the German language
in its largest region, shows stronger digital engagement and significantly higher
purchasing power, making it the highest-ROI market in the analysis.

---

## Analysis Overview

| Step | Method | Business Purpose |
|------|--------|-----------------|
| 1. EDA | KPI calculation, seasonality analysis | Understand baseline performance |
| 2. Conversion Lift | Controlled experiment, Test vs Control | Isolate true incremental impact |
| 3. Statistical Validation | Two-proportion Z-test | Confirm results are not random |
| 4. MMM | Adstock + OLS regression | Estimate long-term channel contribution |
| 5. SQL Analytics | CTEs, Window Functions, CASE WHEN | Surface performance insights |
| 6. Budget Optimization | ROI-based reallocation | Translate findings into action |

---

## Exploratory Data Analysis

![Regional KPIs](images/3_1_kpis.png)
*3-year cumulative performance: Switzerland generates 3.2x more revenue than Germany with the same spend.*

![Seasonality](images/3_2_seasonality.png)
*Q4 drives the strongest revenue across all markets. Switzerland peaks at nearly €58,000/day in December.*

![Funnel](images/3_3_funnel.png)
*Germany's CVR (3.31%) is 51% below Switzerland (5.00%), compounding into large CPA and ROI gaps.*

![Correlation](images/3_4_correlation.png)
*Google spend correlates strongly with traffic (0.97) but weakly with revenue (0.30). ROI is largely independent of spend (0.14).*

---

## Conversion Lift Study

A user-level experiment was simulated across **10,000 users** to isolate the true
incremental impact of ad exposure. Users were randomly assigned to Test and Control
groups, with country-specific conve
