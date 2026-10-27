# 🌍 World Happiness Analytics — Global Socio-Economic Well-Being & Macro Factor Analysis

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=78350F,D97706,FBBF24&height=220&section=header&text=World%20Happiness%20Analytics&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Global%20Socio-Economic%20Well-Being%20%26%20Macro%20Factor%20Analysis&descSize=18&descAlignY=60&descAlign=50" width="100%" alt="World Happiness Analytics Banner" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Domain-Data%20Warehousing%20%26%20Mining-78350F?style=for-the-badge" alt="DWM" />
  <img src="https://img.shields.io/badge/Tool-Microsoft%20Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  <img src="https://img.shields.io/badge/Calculations-DAX%20Measures-D97706?style=for-the-badge" alt="DAX" />
  <img src="https://img.shields.io/badge/Data-CSV%20Dataset-239120?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="CSV" />
  <img src="https://img.shields.io/badge/Documentation-Technical%20Research%20Report-red?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="PDF Report" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License" />
</p>

---

## 📌 Table of Contents

- [📖 Executive Summary](#-executive-summary)
- [🎯 Research Objectives & Dataset Scope](#-research-objectives--dataset-scope)
- [✨ Key Features & Macroeconomic Insights](#-key-features--macroeconomic-insights)
- [📊 Power BI Dashboard Architecture](#-power-bi-dashboard-architecture)
- [📐 Key DAX Measures & Formulations](#-key-dax-measures--formulations)
- [📁 Project Structure](#-project-structure)
- [⚙️ How to Explore the Dashboard & Reports](#️-how-to-explore-the-dashboard--reports)
- [👩‍💻 Author & Academic Context](#-author--academic-context)

---

## 📖 Executive Summary

The **World Happiness Analytics & DWM Intelligence Portfolio** is a comprehensive Data Warehousing and Mining (DWM) research study evaluating the macroeconomic, institutional, and social determinants of international life satisfaction. Centered around the United Nations Sustainable Development Solutions Network dataset, the repository pairs an interactive **Microsoft Power BI Dashboard** (`.pbix`) with a formal academic research report (`Keerthi.N_World_Happiness_Report2024(DWM).pdf`) analyzing how GDP per capita, social safety nets, healthy life expectancy, personal freedom, generosity, and public corruption interact to shape national happiness scores.

---

## 🎯 Research Objectives & Dataset Scope

- **Dataset Source:** World Happiness Report 2024 indicators spanning 140+ countries and sovereign territories.
- **Primary Research Question:** To what degree do economic factors (log GDP) predict self-reported life satisfaction relative to subjective institutional variables (freedom of choice, public trust, perceived corruption)?
- **Analytical Scope:** Multidimensional correlation matrices, regional cohort clustering (Nordic, Western Europe, Sub-Saharan Africa, South Asia), and variance decomposition across the Cantril Ladder index.

---

## ✨ Key Features & Macroeconomic Insights

- **💰 Economic Diminishing Returns:** While GDP per capita strongly correlates with happiness in developing economies, the correlation plateaus in high-income states where personal freedom and social support become dominant factors.
- **🛡️ Social Safety Net Resilience:** Countries with high social support scores exhibit greater happiness stability during macroeconomic shocks.
- **🏛️ Corruption Perception Impact:** Low perceived public corruption acts as a critical multiplier for civic contentment across top-ranking nations.
- **📊 Interactive Power BI Visualizations:** Global choropleth map, regional drill-down slicers, scatter plots with regression trend lines, and KPI cards.

---

## 📊 Power BI Dashboard Architecture

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                 World Happiness Power BI Analytical Schema                  │
└─────────────────────────────────────────────────────────────────────────────┘
                                       │
                                       ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│ Source Layer: World-happiness-report-2024.csv                               │
│ (Ladder Score, Log GDP, Social Support, Life Exp, Freedom, Corruption)      │
└──────────────────────────────────────┬──────────────────────────────────────┘
                                       │
                                       ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│ Transformation Layer: Power Query (M Language)                              │
│ - Schema normalization, country code standardisation, regional grouping     │
└──────────────────────────────────────┬──────────────────────────────────────┘
                                       │
                                       ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│ Semantic & Calculation Layer: DAX Measure Formulations                      │
│ - Global Average Ladder Score                                               │
│ - Regional Rank Indices                                                     │
│ - Factor Contribution Weight %                                              │
└──────────────────────────────────────┬──────────────────────────────────────┘
                                       │
                                       ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│ Presentation Layer: Power BI Interactive Report (`.pbix`)                   │
│ ┌─────────────────────────┐ ┌─────────────────────────┐ ┌────────────────┐  │
│ │ Global Choropleth Map   │ │ Factor Correlation Plot │ │ Regional Cards │  │
│ └─────────────────────────┘ └─────────────────────────┘ └────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 📐 Key DAX Measures & Formulations

```dax
// Average National Happiness Score
Avg_Happiness_Score = AVERAGE('World-happiness-report-2024'[Ladder score])

// Factor Contribution to Well-Being
GDP_Contribution_Ratio = 
    DIVIDE(
        SUM('World-happiness-report-2024'[Explained by: Log GDP per capita]),
        SUM('World-happiness-report-2024'[Ladder score]),
        0
    )
```

---

## 📁 Project Structure

```text
World-Happiness-Report/
├── World_Happiness_Report(DWM).pbix              # Interactive Microsoft Power BI dashboard file
├── Keerthi.N_World_Happiness_Report2024(DWM).pdf # Formal academic research and DWM methodology report
├── World-happiness-report-2024 (1).csv           # Global empirical dataset
└── README.md                                     # Production technical documentation
```

---

## ⚙️ How to Explore the Dashboard & Reports

### 1. View the Interactive Power BI Dashboard
1. Install [Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free on Windows).
2. Download or clone this repository:
   ```bash
   git clone https://github.com/keerthi19hub/World-Happiness-Report.git
   cd World-Happiness-Report
   ```
3. Open `World_Happiness_Report(DWM).pbix` in Power BI Desktop to interact with regional filters and choropleth visualizations.

### 2. Read the Formal Academic Report
- Open `Keerthi.N_World_Happiness_Report2024(DWM).pdf` directly in any web browser or PDF reader for the complete research methodology, statistical findings, and bibliography.

---

## 👩‍💻 Author & Academic Context

**Keerthi N**  
- **GitHub:** [@keerthi19hub](https://github.com/keerthi19hub)  
- **Portfolio:** [keerthi19hub.github.io](https://keerthi19hub.github.io)  
- **Course:** Data Warehousing and Mining (DWM) · Alliance University, Bengaluru  
- **Role:** Designed the Power BI star schema, engineered DAX measures, performed econometric correlation analysis, and authored the technical publication report.

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=78350F,D97706,FBBF24&height=100&section=footer" width="100%" alt="Footer Banner" />
</p>
