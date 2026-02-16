<div align="center">

# 📉 Unemployment Analysis with Python
### CodeAlpha Data Science Internship — Task 2

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7+-11557c?style=for-the-badge)](https://matplotlib.org)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.12+-4c8cbf?style=for-the-badge)](https://seaborn.pydata.org)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3+-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Status](https://img.shields.io/badge/Status-✅%20Completed-2ecc71?style=for-the-badge)]()
[![Internship](https://img.shields.io/badge/CodeAlpha-Internship-FF6B6B?style=for-the-badge)]()

<br>

> **A comprehensive unemployment analysis of India (2019–2020)** covering Covid-19 impact, state & zone-wise trends, rural vs urban breakdown, and a polynomial regression forecast — with 9 professional visualizations.

<br>

[📓 View Notebook](#-notebook-preview) • [📊 Key Findings](#-key-findings) • [🚀 How to Run](#-how-to-run) • [📁 Project Structure](#-project-structure)

</div>

---

## 📌 Project Overview

This project is **Task 2** of the CodeAlpha Data Science Internship. It performs a full-scale analysis of unemployment data across India from **May 2019 to October 2020**, with a sharp focus on how the **Covid-19 pandemic and the March 2020 national lockdown** affected employment across all states, zones, and area types (rural/urban).

The analysis answers real policy questions: *Which states were hit hardest? Did cities suffer more than villages? What does the recovery look like?*

---

## 🎯 Objectives

- ✅ Clean, preprocess, and merge two complementary unemployment datasets
- ✅ Perform thorough EDA with monthly, regional, and area-wise visualizations
- ✅ Quantify and visualize the Covid-19 impact on unemployment rates
- ✅ Analyze zone-wise and state-wise trends using heatmaps and comparisons
- ✅ Compare Rural vs Urban unemployment before and after lockdown
- ✅ Build a time series forecast model to project recovery trajectory
- ✅ Derive actionable policy insights from the data

---

## 📂 Datasets

| Dataset | Records | Coverage | Unique Features |
|---------|---------|----------|-----------------|
| `Unemployment_in_India.csv` | 740 | May 2019 – Jun 2020 | Rural/Urban split, 28 states |
| `Unemployment_Rate_upto_11_2020.csv` | 267 | Jan 2020 – Oct 2020 | Zone classification, GPS coordinates |

**Features used across both datasets:**

| Feature | Description |
|---------|-------------|
| `Region` | Indian state name |
| `Date` | Month-end date |
| `Unemployment_Rate (%)` | Primary target variable |
| `Estimated Employed` | Total employed workforce |
| `Labour Participation Rate (%)` | % of working-age population active |
| `Area` | Rural / Urban (Dataset 1 only) |
| `Zone` | North/South/East/West/Northeast (Dataset 2 only) |

---

## 🛠️ Tech Stack

| Tool | Version | Purpose |
|------|---------|---------|
| Python | 3.10+ | Core language |
| Pandas | 2.0+ | Data loading, cleaning, transformation |
| NumPy | 1.24+ | Numerical operations |
| Matplotlib | 3.7+ | Line charts, bar charts, trend plots |
| Seaborn | 0.12+ | Heatmaps, KDE plots |
| Scikit-learn | 1.3+ | Polynomial regression forecasting |
| Jupyter Notebook | — | Development environment |

---

## 🦠 Covid-19 Impact — Key Numbers

| Metric | Value |
|--------|-------|
| Pre-Covid Avg Unemployment | ~7–8% |
| Peak Unemployment (Apr–May 2020) | 📈 Sharply Higher |
| % Increase Post-Lockdown | Significant spike |
| Recovery Start | Jun 2020 onwards |
| Most Affected Zone | East / Northeast India |
| Urban vs Rural | Urban consistently higher |

> 💡 *Exact numbers generated when you run the notebook — results printed in the final summary cell.*

---

## 📊 Key Findings

1. **Covid-19 caused the sharpest unemployment spike in the dataset** — The March 2020 lockdown triggered a dramatic and near-instantaneous rise in unemployment across all states.

2. **Urban unemployment was consistently higher than rural** — India's urban informal workforce (daily-wage, gig workers) bore a disproportionate burden.

3. **Labour Force Participation dropped sharply** — Many workers, especially women, exited the workforce entirely during the lockdown rather than remaining "unemployed."

4. **Recovery was underway by June 2020** — The polynomial regression forecast confirms a declining trend from the peak, though rates remained above pre-Covid levels.

5. **State-level variation is significant** — Some states maintained relatively low rates throughout, while others hit extreme highs — highlighting the need for targeted interventions.

---

## 📈 Visualizations (9 Plots)

| # | Plot | File | Description |
|---|------|------|-------------|
| 1 | 📈 National Trend | `national_trend.png` | Monthly unemployment with Covid shading |
| 2 | 📊 Distribution | `distribution_analysis.png` | Histogram, boxplot by year, Rural vs Urban KDE |
| 3 | 📅 Seasonal Patterns | `seasonal_patterns.png` | Monthly averages + Labour participation trend |
| 4 | 🦠 Covid Impact | `covid_impact.png` | 4-panel deep dive: before/after, workforce drop, state comparison |
| 5 | 🗺️ Zone Analysis | `zone_analysis.png` | Zone trends over time + average by zone bar chart |
| 6 | 🌡️ State Heatmap | `state_heatmap.png` | State × Month unemployment heatmap |
| 7 | 🏆 Best/Worst States | `top_bottom_states.png` | Top 5 highest and lowest unemployment states |
| 8 | 🏘️ Rural vs Urban | `rural_urban_analysis.png` | Rural/Urban trend + pre vs post Covid split |
| 9 | 📈 Forecast | `forecast.png` | Polynomial regression fit + 4-month forecast |

---

## 🏛️ Policy Recommendations

1. **Expand rural job guarantee schemes** (like MGNREGS) automatically during national crises
2. **Portable benefits for urban informal workers** — delink social security from employers
3. **State-specific interventions** for consistently high-unemployment states
4. **Women's workforce re-entry programs** to recover dropped Labour Force Participation
5. **Real-time monthly unemployment dashboards** for faster policy responses

---

## 📁 Project Structure

```
CodeAlpha_UnemploymentAnalysis/
│
├── 📓 unemployment_analysis.ipynb       ← Main Jupyter Notebook
├── 📄 README.md                         ← This file
├── 📋 requirements.txt                  ← Python dependencies
├── 📂 Unemployment_in_India.csv         ← Dataset 1
├── 📂 Unemployment_Rate_upto_11_2020.csv ← Dataset 2
│
└── 📊 Generated Plots/
    ├── national_trend.png
    ├── distribution_analysis.png
    ├── seasonal_patterns.png
    ├── covid_impact.png
    ├── zone_analysis.png
    ├── state_heatmap.png
    ├── top_bottom_states.png
    ├── rural_urban_analysis.png
    └── forecast.png
```

---

## 🚀 How to Run

### Option 1 — Google Colab *(Recommended — No Setup)*

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MOHAMMED-ABUZAR317/CodeAlpha_UnemploymentAnalysis/blob/main/unemployment_analysis.ipynb)

> **Important:** Upload both CSV files when prompted in Colab (or place them in the same folder as the notebook).

### Option 2 — Run Locally

```bash
# 1. Clone the repository
git clone https://github.com/MOHAMMED-ABUZAR317/CodeAlpha_UnemploymentAnalysis.git
cd CodeAlpha_UnemploymentAnalysis

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch notebook
jupyter notebook unemployment_analysis.ipynb
```

---

## 📦 Requirements

```txt
pandas>=2.0.0
numpy>=1.24.0
scikit-learn>=1.3.0
matplotlib>=3.7.0
seaborn>=0.12.0
jupyter>=1.0.0
```

```bash
pip install -r requirements.txt
```

---

## 📚 What I Learned

- How to clean and merge multiple real-world datasets with different structures
- Visualizing time series data with event markers (lockdown dates, shaded periods)
- Quantifying the economic impact of a real-world event (Covid-19) with data
- Building polynomial regression for non-linear time series forecasting
- Translating data insights into actionable policy recommendations

---

## 🔗 Connect

<div align="center">

| Platform | Link |
|----------|------|
| 💼 LinkedIn | [Mohammed Abuzar](https://linkedin.com/in/mohammed-abuzar) |
| 🐙 GitHub | [MOHAMMED-ABUZAR317](https://github.com/MOHAMMED-ABUZAR317) |
| 🏢 Internship | [CodeAlpha](https://www.codealpha.tech) |

</div>

---

<div align="center">

**📉 Made with ❤️ during the CodeAlpha Data Science Internship**

*If you found this project helpful, please give it a ⭐ on GitHub!*

</div>
