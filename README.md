# Global Power Plants Analysis: Energy, Economics, and Emissions

**Authors:**  
Kaiwen (Kevin) Shao

## Abstract
This project examines the relationship between renewable capacity, CO₂ emissions, and policy measures by integrating datasets from the Global Power Plant Database, World Bank, OECD, and IEA. The goal is to determine whether increased renewable capacity is associated with lower CO₂ emissions and to assess the impact of environmental policies on emissions. Both cross-sectional (single-year) and longitudinal (panel) analyses were conducted. The single-year analysis (e.g., 2014) utilized scatter plots with regression lines and K-Means clustering to reveal country profiles. A multi-year panel analysis (2010–2020) employing two-way fixed effects regression provided additional insights, although the low within R² indicated that GDP and policy measures explain only a small fraction of the variation in emissions. These results underscore the complexity of global emissions dynamics and the need for more comprehensive models.

## Introduction
The global energy transition to renewable power is crucial in reducing CO₂ emissions. However, data on power plant capacity, emissions, economic indicators, and policy measures are fragmented across multiple sources. This project addresses the challenge of integrating diverse datasets to explore how renewable capacity, economic performance (measured by GDP), and environmental policies (proxied by ENVTAX) interact to influence CO₂ emissions. The project contributes to the discussion on energy transitions by employing both cross-sectional and longitudinal analyses to identify key trends and clusters among countries.

## Methods
Data from four sources were integrated:
- The **Global Power Plant Database** provided plant-level capacity data, which was used to compute the renewable capacity ratio.
- The **World Bank** supplied economic (GDP) and environmental indicators (CO₂ emissions and energy use).
- **OECD Green Growth** data contributed an environmental tax measure (ENVTAX) as a proxy for policy strength.
- **IEA data** were considered for supplementary energy balance information.

The methodology was implemented in two stages:

1. **Single-Year Analysis (2014):**  
   - Datasets were preprocessed by standardizing country names and merging by the common “country” field.
   - Missing values and outliers were identified and removed.
   - Scatter plots with fitted regression lines were created to examine the relationship between renewable capacity ratio and CO₂ emissions.
   - K-Means clustering was applied to group countries by renewable ratio, GDP, emissions, and policy measures, revealing distinct energy–economy–policy profiles.

2. **Time-Series (Panel) Analysis (2010–2020):**  
   - A multi-year panel dataset was constructed by compiling annual data on CO₂ emissions, GDP, and environmental tax measures.
   - A two-way fixed effects regression was conducted to control for country-specific and time-specific effects, testing whether higher GDP or stronger policies are associated with lower emissions.
   - Line charts were used to visualize the trends in average CO₂ emissions over time.

This comprehensive methodology quantifies how renewable capacity, economic scale, and policy measures contribute to the variation in global CO₂ emissions, both cross-sectionally and longitudinally.

## Experimental Results (Evaluation)
- **Single-Year Analysis:**  
  The analysis revealed a weak correlation between renewable capacity and CO₂ emissions, suggesting that renewables alone do not guarantee lower emissions. Clustering identified distinct country groups, indicating that factors like economic scale and policy intensity also play critical roles.
  
- **Panel Analysis (2010–2020):**  
  The two-way fixed effects regression produced a statistically significant model, but with very low within R² (approximately 1–2%). This implies that while GDP and policy measures have an effect, they explain only a small part of the emission variation. Visualizations demonstrate an increasing trend in average CO₂ emissions until around 2018, followed by a decline, possibly reflecting shifts driven by policy or economic changes.

## Discussion
The findings suggest that the relationship between renewable capacity and CO₂ emissions is complex. The weak correlation in the single-year analysis and the low explanatory power in the panel model indicate that other factors—such as industrial structure, population, and energy mix—may also significantly influence emissions. Although increasing renewable capacity is beneficial, the results underscore the need for comprehensive policies that address multiple aspects of the energy system to effectively reduce global emissions.

## Statement of Contributions
- **Kaiwen (Kevin) Shao:** Led the integration of datasets, performed data cleaning and preprocessing, conducted both single-year and panel analyses, developed visualizations, and drafted the report.

## Conclusion
This project highlights that renewable capacity and environmental policy measures are important, but they alone cannot fully explain global CO₂ emissions. The modest relationships observed indicate that a broader range of factors must be considered for a comprehensive understanding. Future work will focus on incorporating additional variables and multi-year renewable data, along with further refinement of analytical models, to enhance the explanatory power and provide more targeted policy recommendations.

## References
1. World Resources Institute. *Global Power Plant Database*. World Resources Institute, 2020, https://www.wri.org/resources/data-visualizations/global-power-plant-database.
2. Apergis, Nicholas, and James E. Payne. "The Causal Relationship Between Energy Consumption, CO₂ Emissions and Economic Growth in OECD Countries: Evidence from Panel Data Analysis." *Energy Economics*, vol. 32, no. 2, 2010, pp. 341–348.
3. OECD. *Green Growth Indicators*. OECD Publishing, 2017, https://www.oecd.org/greengrowth/.

## Appendix
All relevant code and additional technical details are available in the GitHub repository.