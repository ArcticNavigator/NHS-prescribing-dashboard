# NHS Prescribing Dashboard - Interactive Analysis of £10.54B NHS Primary Care Spending (2025)

**A live, interactive dashboard that explores NHS primary care prescribing across 42 Integrated Care Boards and 5,764 GP practices showing where the NHS spends, where it overspends, and why.**

[![Live Dashboard](https://img.shields.io/badge/▶%20View%20Live%20Dashboard-20B2AA?style=for-the-badge)](https://nhs-prescribing-dashboard.onrender.com)
[![Streamlit](https://img.shields.io/badge/Built%20with-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io)
[![Python](https://img.shields.io/badge/Python-3.13-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)

---

## View the live dashboard

### 👉 [nhs-prescribing-dashboard.onrender.com](https://nhs-prescribing-dashboard.onrender.com)

> The dashboard runs on a free hosting tier and may take 30–60 seconds to wake up on the first visit. After that it is instant.

---

## What is this?

This is an interactive web dashboard that turns **217 million rows of NHS prescribing data** into a clear, explorable story. It analyses the NHS Business Services Authority (NHSBSA) English Prescribing Dataset (EPD SNOMED) for the whole of 2025 and presents the findings across eight chapters, with charts, maps and filters you can explore yourself.

It answers a single question that matters to every NHS budget holder:

> **Where is the NHS overspending on primary care prescribing, and which areas and practices are driving it?**

---

## What you can explore

The dashboard has eight pages:

- **Introduction** - the business question and how the analysis fits together.
- **Chapter 0 - Building the data.** How 12 monthly files became one clean 217-million-row dataset.
- **Chapter 1 - What is the NHS prescribing?** Which drug categories cost the most versus which are prescribed most.
- **Chapter 2 - Where is the money going?** Cost per prescription across 42 ICBs and 7 regions, with interactive maps of England.
- **Chapter 3 - Who is overspending?** GP practices that spend more than their local peers, every month.
- **Chapter 4 - Can we predict overspending?** A machine learning model that flags at-risk practices.
- **Chapter 5 - Can we forecast spikes?** Forecasts of November and December spending for high-risk categories.
- **Chapter 6 - Does time of year explain spikes?** Which drug categories are seasonal, and how regions differ.

---

## Key findings shown in the dashboard

- The NHS spent **£10.54 billion** on primary care prescribing in 2025 across **1.27 billion** prescriptions.
- **NHS Hampshire and Isle of Wight** is the most expensive ICB at £22.14 per prescription; **NHS North West London** is the cheapest at £18.04.
- **288 GP practices** overspend every single month relative to their local peers.
- The cause of geographic cost variation is **prescribing behaviour**, the choice between branded and generic drugs not procurement prices or patient volume.
- A Random Forest model predicts practice-level cost with **95.4% accuracy** and identifies **2,417 at-risk practices**.

---

## Tech stack

- **Streamlit** - the dashboard framework
- **Plotly** - interactive bar charts, line charts, heatmaps and choropleth maps
- **DuckDB** - fast SQL over 217 million rows during the analysis stage
- **pandas** - data handling
- **GeoPandas** - ICB boundary mapping
- **Render** - free-tier hosting

---

## Features

- Interactive maps of England showing cost, total spend, volume and seasonal change by ICB.
- Filterable tables of the top overspending and underspending GP practices by region and ICB.
- A 42-ICB heatmap showing how spending persists across all 12 months.
- Correlation analysis showing all 7 NHS regions move together seasonally.
- Clear "what this tells us" explanations under every chart, written for non-technical readers.

---

## Run it locally

```bash
# Clone the repository
git clone https://github.com/ArcticNavigator/NHS-prescribing-dashboard.git
cd NHS-prescribing-dashboard

# Install dependencies
pip install -r requirements.txt

# Run the dashboard
streamlit run Dashboard/dashboard.py
```

---

## Related repositories

- **Full project** → [NHS-Prescribe-Seek](https://github.com/ArcticNavigator/NHS-Prescribe-Seek) (notebook, dashboard and model together)
- **Prediction model** → [NHS-prescribing-model](https://github.com/ArcticNavigator/NHS-prescribing-model) (upload data, get at-risk practices)

---

## Data source

English Prescribing Dataset (EPD) with SNOMED code - NHS Business Services Authority Open Data Portal: https://opendata.nhsbsa.net/dataset/english-prescribing-dataset-epd-with-snomed-code

---

## Author

Built by **ArcticNavigator**.

---

*Keywords: NHS prescribing dashboard, NHS primary care spending, interactive healthcare dashboard, Streamlit dashboard, NHS data visualisation, ICB prescribing comparison, NHS cost per prescription, England prescribing map, Plotly choropleth NHS, GP practice spending dashboard, NHS EPD SNOMED, healthcare analytics dashboard, public health data England.*
