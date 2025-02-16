# GlobalPlantsDataset

This repository focuses on analyzing and visualizing global power plant data, along with relevant socio-economic and policy factors that influence the energy landscape.

---

## Week 2 Progress

### Literature Review
- **Created and uploaded** a Literature Review that explores *multi-country* research on energy consumption, emissions, and economic trends.
- Emphasized how **policy instruments** (e.g., carbon pricing, renewable incentives) shape national-level energy outcomes across various countries.
- Highlighted **key methodologies** such as panel data approaches, co-integration, and difference-in-differences for policy impact evaluation.

### Data Alignment
- **Refined dataset selection** to integrate:
  1. IEA time-series data  
  2. World Bank’s World Development Indicators (WDI)  
  3. The Global Power Plant Database
- **Outlined steps** to incorporate both *quantitative* (e.g., subsidy levels) and *qualitative* (e.g., policy start dates) information into the analysis.



Stay tuned for **data cleaning**, **exploratory analysis**, and initial **modeling** phases, building on insights from the literature review.

---
## Week 4 Progress

### Overview
This week, I completed the **initial data collection** and **exploratory data analysis (EDA)** steps:
- Merged power plant data with socio-economic indicators (World Bank).
- Calculated total renewables vs. fossil capacities.
- Examined time-series trends for GDP, emissions, and energy use across top countries.

### Key Achievements
- **Cleaned & Merged**: Created a consolidated `country_capacity` table indicating renewable_ratio for ~167 countries.
- **EDA Visualizations**:
  1. **Bar Charts** for top 10 countries by power plant count, plus total capacity by fuel source.
  2. **Pie Chart** showing global renewable vs. non-renewable share.
  3. **Line Plots** demonstrating GDP trends over time for countries with high fossil vs. high renewables.
  4. **Choropleth Map** (Plotly) indicating “Green Majority” vs. “Fuel Majority” countries.
  ```
  plot Green Majority” vs. “Fuel Majority
  ```
  ![Alt text](pics/map.png)

### Next Steps
- **Enhanced Correlation Analysis**: Investigate relationships between GDP, CO₂, and renewable share with regression or correlation tests.
- **Improve Mapping**: Possibly create an animated map over different years if consistent time-series coverage is found.

### Additional Notes
- **File Sizes**: The final merged dataset remains manageable (~under 100 MB), so it can be stored locally and visualized with Python libraries.
- **Repository**: All `.ipynb` notebooks for EDA and final `.csv` merges are pushed to GitHub for version control.
---