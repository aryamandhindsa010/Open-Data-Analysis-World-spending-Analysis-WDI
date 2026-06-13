# Changing Government Budget allocation during current Geopolitical stance

## Overview

The data provided my `WDI` is a great source as it is an aggregation of whole of the world government data that is available on economy, people, status and spending provided by the world Bank and is considered as the most reliable source. The API provided in R i.e. `package(WDI)` is a quick way to get all the needed variables without having to download the data.

> **Note:** This data is intended for educational and research purposes only.
> It is not intended for real financial analysis or interpretation.

---

## Files Included

| File | Description |
|---|---|
| `assignment-4-Aryaman-Dhindsa.qmd` | The quarto file containing the analysis and blog post |
| `data-dictionary.xlsx` | Full data dictionary documenting all variables, types and details |
| `README.md` | This file — describes the dataset, its origin, and how to use it |

---
### Data-dictionary worksheets

- raw —> The raw data pulled directly from the World Bank API, containing all 11 columns across 260+ countries from 2005–2025 before any filtering or transformation.
- world_avg —> GDP-weighted global averages of military, health, and education spending aggregated by year into long format, used to produce the line chart.
- latest_mil —> A single-row-per-country snapshot of the most recent available military spending figure for each country, used to colour the world map.

## Data Origin

- **Source:** World Bank's World development Indicators API
- **Processing:** Only the required variables were taken as needed
- **Population:** This dataset represents the **Aggregation** of government resources of all countries on economy and other development indicators.

---

## Author and Release

| Field | Details |
|---|---|
| **Author** | Aryaman Dhindsa |
| **Institution** | Monash University |
| **Date of Release** | 08th June, 2026 |
| **Licence** | Creative Commons Attribution 4.0 International (CC BY 4.0) |

Under the CC BY 4.0 licence, users are free to share and adapt this data for
any purpose, provided appropriate credit is given. Re-identification of
individuals is strictly prohibited.

---

### Recommended Packages

```r
library(dplyr)    # Data manipulation
library(ggplot2)  # Visualisation
library(tidyr)    # Data reshaping
```
or a single package
```r
library(tidyverse) 
```

### Meta Data

| Attribute | Description |
|------------|------------|
| **Dataset** | World Development Indicators (WDI)[@wdicite] |
| **Source** | World Bank Group |
| **Access Method** | World Bank Data API accessed through the `WDI` package in R |
| **Geographic Coverage** | 260+ countries, territories, and regional aggregates |
| **Granularity** | National level |
| **Temporal Coverage** | 1960–2025 |
| **Frequency** | Annual |
| **Update Frequency** | Quarterly (April, July, September, December) |
| **Regularly Updated** | Yes |
| **Languages Available** | Arabic, English, French, Chinese, Spanish |
| **License** | Creative Commons Attribution 4.0 International (CC BY 4.0) |
| **First Published** | 1 April 2005 |
| **Last Updated** | 8 April 2026 |

### Licencing

Data were obtained from the World Bank Indicators API and are licensed under CC BY 4.0 [@ccby40].

The Creative Commons Attribution 4.0 International license allows users to copy, modify and distribute data in any format for any purpose, including commercial use.

### Data Privacy

It is an aggregation of publicly available data from the governments all across the globe, which means there are no privacy issues.

### Limitation

- The governments do not provide the right figures and consider giving the wrong data for security reasons.

- The data of WDI is only Macro and do not have regional data of countries so there is no possibility of in-depth provisional or state-wise analysis of a country.

- There are a few countries that considers themselves independent but are not considered as a country by the world bank, all those countries are not included.

- Countries that do not acknowledge the world bank as the world's bank are not included.

- The data for unacknowledged countries is limited or not present.
(All this limitations are considered after assuming that there are no bias due to the amount of funding received by World bank by a particular country. These biases are common as from a geopolitical standpoint.)