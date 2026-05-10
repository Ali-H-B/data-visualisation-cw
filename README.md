# ChrisCo Venue Analytics — Data Visualisation

A visual data exploration of visitor patterns across 35 UK venues for ChrisCo, a fictional venue management company. Built in Python using Google Colab.

## Overview

The project investigates a full year of daily visitor data alongside venue attributes (age, spend, distance, duration, gender split) to surface meaningful patterns and support business decision-making.

Key areas explored:
- **Volume segmentation** — venues categorised into Very High / High / Medium / Low / Very Low tiers based on total annual visitors, identified through visual inspection of the distribution rather than arbitrary quantiles
- **Seasonal & temporal patterns** — rolling average line plots used to compare trends across high-volume venues over time
- **Composition analysis** — stacked area charts showing how the visitor mix shifts across the year
- **Autocorrelation** — detection of weekly and seasonal periodicity across individual venues
- **Venue lifecycle** — identification of venues that opened or closed during the period using activity boundary thresholds
- **Anomaly detection** — flagging of outlier days (>3 standard deviations from venue mean) and unusual venue behaviour
- **Correlations** — scatter plots and heatmaps linking venue attributes (spend, age, distance) to visitor volume
- **Interactive exploration** — ipywidgets-based tools allowing dynamic filtering and drill-down by venue segment

## Tech Stack

- Python (pandas, NumPy, matplotlib, seaborn, ipywidgets)
- Google Colab
- Data: 6 CSV files compiled into two dataframes (one row per date; one row per venue)

## Structure

The notebook is organised into clearly documented sections, each with markdown explaining the purpose and rationale of the code that follows. Visualisation choices reference the specific course examples they were adapted from.

## Running the Notebook

1. Open in Google Colab
2. Upload the data ZIP file when prompted (or mount Google Drive)
3. Run all cells in order

> **Note:** Static visualisations render directly on GitHub. The two interactive widgets (built with ipywidgets) require a live kernel to function — open the notebook in Colab or Jupyter to use them.
