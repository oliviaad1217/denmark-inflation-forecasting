Comparing ARIMA and ETS forecasts for Denmark’s monthly inflation using R, chronological evaluation, and residual diagnostics.
# Denmark Inflation Forecasting: ARIMA vs ETS

## Overview

This project compares ARIMA and Exponential Smoothing (ETS)
for forecasting Denmark’s monthly year-over-year inflation rate.

The study uses 240 monthly observations from January 2005
to December 2024. Models are trained on 2005–2023 data
and evaluated against the 12 months of 2024.

## Tools and Methods

- R
- forecast, tseries, strucchange, and ggplot2
- Time-series decomposition
- Stationarity and structural-break analysis
- ARIMA and ETS forecasting
- Residual diagnostics and forecast accuracy evaluation

## Reported Results

| Model | RMSE | MAE |
|---|---:|---:|
| ARIMA | 0.33 | 0.27 |
| ETS | 0.97 | 0.85 |

Errors are expressed in percentage points.

The submitted report finds that ARIMA performs better
on the 2024 holdout period. These are historical reported
results and have not been independently reproduced
for this repository.

## Limitations

- Evaluation covers one 12-month holdout period.
- Structural changes may affect future forecast performance.
- Narrow prediction intervals do not establish reliable coverage.
- The current script uses training-only models for accuracy
  evaluation but full-series models for interval-width comparisons.
  These sections need alignment before interpreting them together.

## Data and Reproduction

The study uses Statistics Denmark data referenced as PRIS111.

The script currently expects a local CSV input. Before running,
obtain the matching series and period, update the input path,
and install the required R packages.

The exact data selection and download instructions should
be documented alongside the input file.



Olivia Liang
Copenhagen Business School
