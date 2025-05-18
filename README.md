# Similar Trading Days Identifier

## Overview

This repository contains the analysis and modeling performed for the Energia Analyathon Challenge. The primary objective was to identify similar trading days based on historical data involving Wind Generation, Energy Demand, and Net Energy Demand across three regions: All Island (AI), Northern Ireland (NI), and the Republic of Ireland (IE).

## Objectives

* Calculate and analyze Net Demand, defined as the difference between Total Demand and Total Generation from renewable sources.
* Create a consistent "Trading Day" timeframe from 23:00 of the previous day to 22:59 of the current day, facilitating precise 30-minute interval price bidding.
* Develop methods to identify similar trading days using clustering and similarity algorithms.

## Data Pre-processing

* Computed Net Demand for AI, NI, and IE.
* Defined and validated "Trading Day" to ensure accurate data segmentation.
* Prepared data at 30-minute intervals for detailed granularity.
* Used Python (Jupyter Notebook) for cleaning and pre-processing tasks.

## Exploratory Data Analysis (EDA)

* Conducted comprehensive visual analysis on Wind Generation, Energy Demand, and Net Energy Demand.
* Observed clear seasonal and hourly trends impacting energy generation and consumption.
* Noted weekly variations in energy usage and production patterns.

## Approaches Used

1. **Daily Aggregation**: Aggregated data daily, simplifying overall trend analysis but potentially missing intraday patterns.
2. **30-Minute Aggregation (Chosen Method)**: Preserved detailed intra-day trends, optimized for similarity analysis.
3. **Segmented Day-Part Aggregation**: Condensed dataset further but did not significantly enhance performance.

## Similarity Identification Methods

* **Cosine Similarity**: Used for its intuitive nature, measuring similarity based on data patterns rather than magnitude alone.
* **KMeans + Cosine Similarity (Recommended)**: Combined clustering (KMeans) for initial data grouping and Cosine Similarity for detailed within-cluster comparisons, improving accuracy.

## Recommendations

* **Wind Generation Optimization**: Leverage identified patterns to enhance scheduling and maintenance.
* **Infrastructure Resilience**: Strengthen capacity to handle fluctuations effectively.
* **Enhanced Load Forecasting**: Use similarity analysis outcomes to improve forecasting precision.
* **Energy Conservation Incentives**: Offer discounts or incentives during low supply periods to encourage reduced consumption.

## Technologies and Tools

* Python
* Jupyter Notebook
* KMeans Clustering
* Cosine Similarity Algorithm
* MinMaxScaler for data normalization

## References

* Hao et al. (2019). *Renewable Energy.*
* Petitjean et al. (2011). *Pattern Recognition.*
* Dabbura (2018). Medium Article on K-Means Clustering.

---

For further details or to reproduce the analysis, refer to the Jupyter notebooks and data files included in this repository.
