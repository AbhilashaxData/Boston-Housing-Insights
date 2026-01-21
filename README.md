# 🏙️ Boston Housing: Socio-Economic Determinants & Market Insights
### Predictive Analytics | Problem Set 1

---

This repository contains a structural exploratory analysis of the **Boston Housing Dataset**. By integrating **Hedonic Pricing Theory** with predictive analytics, this study examines how localized "disamenities" such as pollution, crime, and economic distress are capitalized into urban land values.

## 📊 Project Overview
The analysis utilizes the `MASS` library in **R** to examine 506 rows depicting suburbs across the Boston metropolitan area. Each row represents a specific suburb, while the 14 variables capture the socio-economic, environmental, and institutional characteristics of the region.

## 📂 Repository Contents
* `predictive_analysis_pset1.Rmd`: Source R Markdown file containing the complete analysis pipeline.
* `predictive_analysis_pset1.docx`: Final report knitted in word document.

---

## 🧪 Key Research Insights

1) **📊 Hedonic Pricing & Capitalization (LSTAT vs MEDV)** :
  The inverse relationship between the percentage of "lower status" residents (`lstat`) and median home values (`medv`) illustrates the **capitalization** of neighborhood socio-economics into land values. Framed within **Hedonic Pricing Theory**, housing acts as a **normal good** where localized economic deprivation represents a significant disamenity, resulting in a contraction of demand and a downward shift in equilibrium property prices.

2) **🌱 Environmental Externalities & Market Valuation (NOX vs MEDV)** :
  Nitrogen oxide concentration (`nox`) serves as a proxy for localized **negative externalities**. The observed negative correlation suggests that clean air is a "local public good" for which households exhibit a high **willingness to pay (WTP)**. In localities where environmental degradation is high, property values are discounted, reflecting the market's internal pricing of environmental disamenities.

3) **🏚️ The Structural Poverty Trap** :
By isolating the suburb with the absolute minimum valuation , we observe a convergence of extreme distress markers:
  * **Crime Rate (`crim`):** 98.8th percentile.
  * **Status (`lstat`):** 97.8th percentile.
  
  This identifies a **spatial poverty trap** where cumulative negative externalities (social, economic, and environmental) cause land rents to collapse to a structural lower bound.

4) **⚖️ Institutional Variance & Public Good Provision** :
  Using **outlier detection**, we identified **66 suburbs** with exceptionally high crime rates, indicating that safety is a geographically concentrated public good in the Boston area. Conversely, the variance in **Pupil-Teacher Ratios (`ptratio`)** and **Tax Rates (`tax`)** highlights a sharp divide in resource allocation and fiscal policy, further segmenting the urban housing market.

---

## 🛠️ Technical Implementation
* **Language:** R
* **Library:** `MASS` (Boston Housing Data)


---
