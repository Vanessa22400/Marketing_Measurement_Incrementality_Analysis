# Marketing Measurement & Incrementality Analysis - DACH Region

*End-to-end marketing measurement simulation for a DACH-region e-commerce company using Conversion Lift studies, MMM calibration, statistical testing and ROI optimization.*

**Dataset**: Simulated multi-channel marketing dataset (12 months of operations)
**Techniques**: EDA, hypothesis testing, Conversion Lift, MMM, SQL analysis
**Key Result**: Google Ads showed the strongest measurable incremental contribution and Switzerland demonstrated the highest ROI efficiency

---

## Business Context

Modern marketing measurement has become increasingly complex due to:

* privacy restrictions,
* tracking limitations,
* cookie loss,
* fragmented attribution.

As a result, organizations can no longer rely only on traditional attribution models to evaluate marketing performance.

This project simulates how a modern measurement consulting team could evaluate advertising effectiveness for an e-commerce company operating across the DACH region:

* Germany
* Austria
* Switzerland

The objective is to understand whether marketing investments are truly generating incremental business growth and how ROI can be optimized across channels and regions.

---

## Dataset

The project uses a simulated marketing dataset representing 12 months of campaign activity across multiple channels.

The dataset includes:

* Google Ads investment
* Meta Ads investment
* TV investment
* Influencer Marketing investment
* impressions
* clicks
* conversions
* revenue
* seasonal indicators
* regional segmentation

The project intentionally simulates realistic business behavior, including:

* seasonal demand peaks,
* regional differences,
* saturation effects,
* delayed advertising impact.

---

## Problem Statement

How can a company accurately measure the real business impact of advertising investment in a privacy-limited environment?

The project focuses on three core measurement challenges:

* isolating incremental impact,
* estimating channel contribution,
* optimizing ROI allocation.

---

## Objectives

* Analyze marketing performance across DACH markets
* Understand regional differences in ROI and incrementality
* Simulate a Conversion Lift experiment using control and test groups
* Validate statistical significance of marketing uplift
* Build a simplified Marketing Mix Model (MMM)
* Simulate Adstock and saturation effects
* Compare channel contribution across media types
* Perform SQL-style ROI analysis
* Generate strategic optimization recommendations

---

## Methodology

1. **Data Preparation & Feature Engineering**
2. **Exploratory Data Analysis (EDA)**
3. **Seasonality & Regional Analysis**
4. **Conversion Lift & Incrementality Analysis**
5. **Hypothesis Testing & Statistical Significance**
6. **Marketing Mix Modeling (MMM)**
7. **Adstock & Saturation Modeling**
8. **MMM Calibration**
9. **SQL-based ROI Analysis**
10. **Strategic Budget Optimization**

---

## Tools & Technologies

* Python (Pandas, NumPy)
* Scikit-learn
* SciPy (Hypothesis Testing)
* Statsmodels
* Matplotlib & Seaborn
* SQL / BigQuery-style aggregation
* Marketing Mix Modeling concepts
* Incrementality & Lift methodology

---

## Exploratory Data Analysis Highlights

The exploratory analysis revealed several important business patterns:

* **Germany generated the highest overall business volume**, but also showed signs of stronger saturation and lower relative efficiency.
* **Switzerland demonstrated the strongest ROI efficiency**, despite lower total scale.
* **Austria presented stable intermediate performance** across most KPIs.
* Strong seasonal effects appeared between November and December, likely influenced by Black Friday and holiday shopping behavior.
* Revenue dropped significantly after the holiday period, suggesting a clear post-holiday demand effect.

These findings reinforced the importance of regional measurement strategies instead of relying only on aggregated metrics.

---

## Conversion Lift & Incrementality Analysis

A simulated Conversion Lift experiment was developed using:

* control group,
* test group,
* user-level split design.

The objective was to estimate incremental impact by measuring whether users converted because of advertising exposure or whether they would likely convert naturally.

### Key findings

* Test groups consistently outperformed control groups across all regions.
* Statistical testing confirmed that the uplift was statistically significant ("StatSig").
* Switzerland demonstrated the strongest relative Lift performance.
* Germany demonstrated larger scale but lower relative incremental efficiency.

The project also explored how regional consumer behavior may influence campaign responsiveness and advertising trust.

---

## Marketing Mix Modeling (MMM)

A simplified MMM framework was implemented to estimate channel contribution using aggregated time-series data.

The project included:

* baseline demand estimation,
* media contribution modeling,
* Adstock transformation,
* saturation analysis.

### Key findings

* Google Ads showed the strongest measurable contribution.
* Influencer Marketing also demonstrated strong estimated impact.
* Meta Ads presented weaker contribution in the simulated environment.
* TV investment showed lower measurable incremental efficiency and possible saturation effects.

---

## Adstock & Saturation Effects

The project simulated delayed advertising impact through Adstock modeling.

This approach reflects how advertising influence may persist over time instead of disappearing immediately after exposure.

Saturation analysis also demonstrated diminishing returns, suggesting that additional investment may eventually generate progressively smaller incremental gains.

These concepts are highly relevant in modern marketing measurement and media optimization.

---

## SQL & ROI Analysis

SQL-style aggregation using BigQuery-inspired syntax was used to calculate:

* regional ROI,
* conversion performance,
* revenue contribution,
* investment efficiency.

### Regional ROI findings

| Country     | ROI Performance                             |
| ----------- | ------------------------------------------- |
| Switzerland | Highest ROI efficiency                      |
| Austria     | Stable intermediate ROI                     |
| Germany     | Highest scale but lower relative efficiency |

These results reinforced the importance of balancing scale and efficiency during strategic allocation decisions.

---

## Strategic Optimization Recommendations

Based on:

* Lift studies,
* MMM contribution,
* saturation signals,
* ROI analysis,

the project simulated an optimization scenario suggesting:

* increased investment in Google Ads,
* increased allocation to Influencer Marketing,
* reduced TV allocation,
* stronger focus on high-efficiency regional opportunities.

---

## Business Impact & Applications

This project demonstrates how modern organizations can combine:

* experimentation,
* causal inference,
* statistical modeling,
* marketing analytics,
* ROI optimization

to improve measurement reliability and strategic decision-making.

Potential applications include:

* media planning,
* budget optimization,
* incrementality measurement,
* campaign calibration,
* regional strategy development.

---

## Limitations

* The dataset is simulated and simplified for educational purposes.
* External variables such as macroeconomic conditions and competitor actions are not included.
* MMM was implemented using a simplified regression-based approach instead of enterprise-scale Bayesian frameworks.

---

## Next Steps

* Integrate Bayesian MMM approaches (LightweightMMM)
* Add customer segmentation analysis
* Simulate attribution window differences
* Expand cross-device and privacy-safe measurement scenarios
* Build an interactive marketing performance dashboard

---

## Repository Structure

```bash
.
├── data
├── notebooks
├── images
├── requirements.txt
└── README.md
```

---

## Strategic Perspective

This project was intentionally designed to simulate how modern marketing measurement teams combine experimentation, statistical modeling and business strategy to evaluate advertising effectiveness.

Rather than relying only on attribution metrics, the analysis focuses on understanding incremental business impact, regional behavior differences and the limits of measurement in privacy-constrained environments.

The project also reflects an international perspective by incorporating regional dynamics across Germany, Austria and Switzerland.

---

## Conclusion

This project simulates a modern end-to-end measurement framework for evaluating marketing effectiveness across the DACH region.

The analysis combines:

* Conversion Lift studies,
* Incrementality analysis,
* MMM calibration,
* ROI optimization,
* statistical validation,
* strategic regional analysis

to better understand how advertising investment contributes to measurable business growth.

A key takeaway is that modern marketing measurement increasingly depends on combining experimentation and statistical modeling rather than relying only on traditional attribution systems.
