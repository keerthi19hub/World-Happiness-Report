# World Happiness Report 2024 — Data Analytics & Power BI Dashboard

> **A Data Warehousing & Mining (DWM) analytical project examining global wellbeing indicators through interactive Power BI dashboards, econometric correlation analysis, and formal research documentation.**

[![Power BI](https://img.shields.io/badge/BI-Power%20BI-F2C811?logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![Data Analytics](https://img.shields.io/badge/Domain-Global%20Wellbeing%20Analytics-blue)](https://github.com/keerthi19hub)
[![DWM](https://img.shields.io/badge/Subject-Data%20Warehousing%20%26%20Mining-green)](https://github.com/keerthi19hub)

---

## 1. Project Overview

The **World Happiness Report 2024 Analysis** is a comprehensive Data Warehousing & Mining (DWM) academic research project that investigates the measurable socioeconomic and institutional drivers of population-level happiness and wellbeing across nations.

Using official 2024 World Happiness Report data (157 countries), the project delivers:
- **Multi-dimensional statistical correlation analysis** between happiness scores and economic/social indicators.
- **Interactive Power BI dashboards** with geographic heat maps, KPI scorecards, and trend visuals.
- **Formal DWM technical research report** documenting methodology, hypothesis tests, and findings.

---

## 2. Dataset Overview

**Source:** World Happiness Report 2024 (`World-happiness-report-2024 (1).csv`)

| Feature / Indicator | Description | Analytical Role |
| :--- | :--- | :--- |
| **Life Ladder** *(Happiness Score)* | Cantril Ladder subjective wellbeing score (0–10 scale) | Primary target variable |
| **Log GDP per Capita** | Natural log of GDP per capita (PPP, constant 2017 USD) | Economic prosperity proxy |
| **Social Support** | Perceived availability of social support network | Social cohesion indicator |
| **Healthy Life Expectancy at Birth** | Life expectancy adjusted for years lived in good health | Health and welfare indicator |
| **Freedom to Make Life Choices** | Perceptions of autonomy and personal agency | Governance quality indicator |
| **Generosity** | Residual of donations relative to GDP | Social capital indicator |
| **Perceptions of Corruption** | Perceived corruption in business and government | Institutional trust indicator |
| **Positive / Negative Affect** | Prevalence of positive vs. negative emotional experiences | Psychological wellbeing |
| `year` | Survey collection year (allows temporal trend analysis) | Temporal control variable |

---

## 3. Analytical Framework & Key Findings

### 3.1 Country Rankings (2024 Highlights)
- **Top Performers:** Nordic nations (Finland, Denmark, Iceland, Sweden) consistently dominate rankings, driven by high social support, strong health systems, and low corruption.
- **Regional Insights:** Sub-Saharan African nations cluster at lower scores, predominantly correlated with GDP per capita deficits and social support gaps.

### 3.2 Econometric Correlations Analyzed
| Indicator Pair | Correlation Insight |
| :--- | :--- |
| GDP per Capita ↔ Happiness | Strong positive correlation; diminishing returns above a threshold |
| Social Support ↔ Happiness | Among the highest individual correlations across all indicators |
| Freedom of Choice ↔ Happiness | Significant in both high-income and middle-income nations |
| Perceptions of Corruption ↔ Happiness | Strong negative correlation — lower corruption = higher happiness |

### 3.3 Power BI Dashboard Features
- **Global Choropleth Map:** Country-level happiness score coloring for instant geographic pattern recognition.
- **Indicator Scatter Plots:** Bivariate relationship visualization between happiness and each sub-index.
- **Year-over-Year Trends:** Temporal tracking of regional average happiness across survey years.
- **KPI Scorecards:** Top/Bottom 10 country rankings with drill-through detail cards.

---

## 4. Repository Structure

```
World-Happiness-Report/
├── World-happiness-report-2024 (1).csv          # Official WHR 2024 dataset (157 countries)
├── World_Happiness_Report(DWM).pbix             # Interactive Power BI dashboard file
├── Keerthi.N_World_Happiness_Report2024(DWM).pdf # Full DWM technical research report
└── README.md                                     # Project documentation
```

---

## 5. Usage & Exploration

### Opening the Power BI Dashboard
1. Install **[Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/)** (free).
2. Open `World_Happiness_Report(DWM).pbix`.
3. Use the **Region**, **Year**, and **Country** slicers to explore filtered views.
4. Drill through country cards for full sub-indicator breakdowns.

### Reading the Research Report
- Open `Keerthi.N_World_Happiness_Report2024(DWM).pdf` in any PDF reader.
- The report documents the problem statement, methodology, data transformations, analytical outputs, and recommended policy implications.

---

## 6. Technology Stack

- **Data Modeling & Visualization:** Microsoft Power BI (`.pbix`), DAX
- **Data Format:** CSV (157 countries × 9 dimensions × multiple survey years)
- **Documentation:** Formal technical report (PDF)

---

## 7. Author & Academic Context

- **Author:** **Keerthi N** (*Alliance University, BCA*)
- **Subject:** Data Warehousing & Mining (DWM)
- **Verified Contribution:** Authored the full DWM technical research report, built the interactive Power BI data model with DAX measures, and produced all analytical visualizations.

---

## 8. Data Attribution

- **Original Dataset:** [World Happiness Report](https://worldhappiness.report/) — Gallup World Poll.
- **This analysis** is independently developed as academic coursework at Alliance University.

---

## 9. License

Released under the [MIT License](https://opensource.org/licenses/MIT).
