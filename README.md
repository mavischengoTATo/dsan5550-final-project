# dsan5550-final-project
# Predicting Parent Company Stock Prices Based on Facility Carbon Emissions and Local Climate Data

## Project Overview

This project explores the complex relationship between regional climate conditions around factories and the daily stock prices of their parent companies. We hypothesize that local climate variables can serve as indicators of factory operational efficiency and affect production efficiency, business performance, and ultimately stock prices.

## Data Sources

Our study aims to thoroughly examine the impact of environmental factors on corporate financial performance, leveraging data from three principal sources:
1.   [Climate Data from Meteostat](https://github.com/meteostat/meteostat-python?tab=readme-ov-file)

*   We source our primary climate data from Meteostat, which provides a simple API for accessing comprehensive historical weather and climate data. The data is aggregated from various public sources, including national weather services such as the National Oceanic and Atmospheric Administration (NOAA) and Germany's national meteorological service (DWD). This dataset includes detailed observations that are essential for analyzing climate variables relevant to the geographic locations of the facilities under study. The integration with OpenCage Geocoder allows us to convert facility ZIP codes into precise geographical coordinates, ensuring the selection of appropriate nearby weather stations from Meteostat’s extensive database.
2.   [Carbon Emissions Data from GHGRP](https://www.epa.gov/ghgreporting/find-and-use-ghgrp-data)

*   Carbon emissions data are obtained from the Environmental Protection Agency’s Greenhouse Gas Reporting Program (GHGRP). This comprehensive dataset details emissions by type and process for significant emission facilities in the U.S., along with information about their highest-level parent companies. It allows us to link emissions data directly to corporate entities and analyze the environmental impact of specific facilities.

3.   [Financial Data from Yahoo Finance](https://developer.yahoo.com/api/)
*    Financial performance data, including daily stock prices, is sourced using the Yahoo Finance API. This dataset includes transactions from 2022 and covers 364 parent companies with 3,733 facilities listed in Carbon Emissions Data from GHGRP. All companies and associated Exchange-Traded Funds (ETFs) are U.S.-based and listed on the U.S. stock market. These stock prices are essential for evaluating the financial implications of environmental performance and changes.
4. [Risk-free Rate from U.S. Department of the Treasury](https://home.treasury.gov/resource-center/data-chart-center/interest-rates/TextView?type=daily_treasury_real_long_term&field_tdr_date_value=2022)
* In the CAPM model, we utilize Daily Treasury Real Long-Term Rates as the risk-free rate instead of a standard risk-free rate.

