# NYC Urban Heat & Environmental Vulnerability Analysis (2022–2025)
Geospatial analysis of persistent urban heat and environmental vulnerability across 197 NYC neighborhoods (2022-2025).

### A Geospatial Data Analytics & Urban Climate Resilience Project

## Project Overview

This independent research project investigates persistent summer land surface temperature (LST) patterns across New York City from 2022 to 2025.

Using satellite remote sensing, geospatial analysis, and socioeconomic data, the project examines how urban heat relates to vegetation, impervious surfaces, poverty, and older-adult populations.

The goal is to identify neighborhoods where persistent surface heat overlaps with selected socioeconomic vulnerabilities, providing a data-driven screening framework for green infrastructure assessment and climate-resilience planning.

**Geographic Scope:** New York City, 197 standard Neighborhood Tabulation Areas (NTAs)

**Study Period:** Summer 2022–2025

**Tools:** Python, Google Earth Engine, Google Colab, GeoPandas, Pandas, Matplotlib, GIS

## Research Questions

1. Which NYC neighborhoods experienced persistently elevated summer surface temperatures?
2. How do vegetation and impervious land cover relate to neighborhood surface temperatures?
3. Where do persistent urban heat and socioeconomic vulnerability overlap?
4. How sensitive are the results to changes in permanent-water masking?

## Data Sources

| Dataset | Purpose |
|---|---|
| Landsat 8 & 9 Collection 2 Level-2 | Summer land surface temperature and vegetation analysis |
| NYC 2020 Neighborhood Tabulation Areas | Geographic boundaries |
| U.S. Census ACS 2024 5-Year Estimates | Poverty and older-adult population indicators |
| National Land Cover Database (2021) | Impervious surface coverage |
| JRC Global Surface Water | Original water masking |
| ESA WorldCover | Additional permanent-water mask validation |

## Methodology

**1. Satellite Data Processing**

Processed Landsat 8 and 9 satellite imagery using Google Earth Engine to estimate summer land surface temperatures for June through August, 2022–2025.

Applied cloud and quality masking, generated monthly temperature composites, and aggregated measurements to neighborhood boundaries.

**2. Environmental and Socioeconomic Integration**

Combined neighborhood temperature measurements with NDVI, impervious surface percentages, poverty rates, and the proportion of residents aged 65 and older.

**3. Persistent Hotspot Identification**

Classified neighborhoods as persistent heat hotspots when they ranked within the hottest 25% during at least three of four summers.

**4. Priority Neighborhood Screening**

Identified priority neighborhoods where persistent heat overlapped with poverty or older-adult population shares at or above the 75th percentile.

**5. Statistical and Spatial Analysis**

Used descriptive statistics, Spearman correlations, and geospatial visualizations to investigate environmental relationships and neighborhood-level differences.

**6. Sensitivity Validation**

Tested an additional permanent-water mask across all four years to assess whether water classification affected temperature estimates and persistent-hotspot identification.

## Key Findings

- **197 NYC neighborhoods** analyzed.
- **36 persistent heat hotspots** identified.
- **14 priority neighborhoods** identified where persistent surface heat overlaps with selected socioeconomic vulnerabilities.
- Persistent hotspots averaged **40.54°C**, compared with **38.38°C** in other neighborhoods.
- Persistent hotspots had higher average impervious cover (82.87% versus 77.73%) and lower NDVI (0.262 versus 0.297).
- Spearman correlations with summer LST were +0.283 for impervious cover, −0.238 for NDVI, +0.182 for poverty, and −0.171 for older-adult population share.
- A four-year water-mask sensitivity analysis produced mean absolute temperature changes of approximately 0.03°C annually, with **no changes to persistent-hotspot classifications**.

## Selected Priority Neighborhoods

| Neighborhood | Borough | Average summer LST |
|---|---|---|
| Queens Village | Queens | 41.11°C |
| East Flatbush-Farragut | Brooklyn | 41.05°C |
| East Williamsburg | Brooklyn | 41.03°C |
| Borough Park | Brooklyn | 41.00°C |
| Flatlands | Brooklyn | 40.63°C |
| Cambria Heights | Queens | 40.62°C |
| Hunts Point | Bronx | 40.60°C |
| South Williamsburg | Brooklyn | 40.52°C |
| Westchester Square | Bronx | 40.40°C |
| Midwood | Brooklyn | 40.20°C |
| East Flatbush-Rugby | Brooklyn | 40.18°C |
| Claremont Village-Claremont (East) | Bronx | 40.17°C |
| Mott Haven-Port Morris | Bronx | 40.05°C |
| East Flushing | Queens | 39.52°C |

## Planning Implications

The results can help guide further assessment of:

- Urban tree canopy expansion and pedestrian shade.
- Cool roofs and reflective surface strategies.
- Heat-resilience infrastructure near vulnerable populations.
- Neighborhood-specific green infrastructure opportunities.
- Equitable climate adaptation and infrastructure investment.

**Important:** Priority neighborhoods are screening candidates, not confirmed optimal locations for specific infrastructure investments. Site-level feasibility, costs, and potential intervention effectiveness require additional analysis.

## Limitations

- Satellite land surface temperature is not equivalent to ambient air temperature or individual heat exposure.
- Neighborhood averages may conceal localized temperature differences.
- Socioeconomic and environmental datasets represent different reference periods.
- Correlations describe associations, not causal relationships.
- The water-mask sensitivity test evaluates one methodological choice rather than all sources of uncertainty.

## Project Deliverables

- Google Colab notebook containing the analytical workflow.
- NYC summer surface temperature and priority neighborhood maps.
- Environmental correlation and neighborhood comparison visualizations.
- Four-year water-mask sensitivity validation.
- Research report and portfolio case study.

## Author

Independent research project focused on applying data analytics, geospatial technologies, and urban sustainability principles to climate-resilience challenges.

## Data Sources

This project integrates publicly available satellite imagery, environmental land-cover datasets, geographic boundaries, and socioeconomic indicators.

| Data Source | Purpose |
|---|---|
| Landsat 8/9 Collection 2 Level-2 | Summer land surface temperature and vegetation analysis, 2022–2025 |
| NYC Neighborhood Tabulation Areas (2020) | Geographic boundaries for 197 neighborhoods |
| U.S. Census ACS 2024 5-Year Estimates | Poverty rates and population aged 65+ |
| National Land Cover Database (2021) | Impervious surface coverage |
| JRC Global Surface Water | Water masking in the primary analysis |
| ESA WorldCover | Additional permanent-water masking for sensitivity validation |

Satellite imagery was processed using Google Earth Engine. Environmental and socioeconomic indicators were integrated at the neighborhood level using Python and geospatial analysis.

**Data considerations:** These datasets represent different collection periods. Satellite-derived land surface temperature measures surface conditions rather than ambient air temperature, and neighborhood-level relationships should not be interpreted as causal effects.
