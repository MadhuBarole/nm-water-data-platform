# USGS Daily Water Summary (Notebook)

## Which source you selected
This notebook uses the USGS Water Data OGC API (daily values endpoint). I chose it because it is an authoritative, public source for hydrologic data and provides consistent daily observations.

## What data you retrieved
- **Location:** Rio Grande at Albuquerque, NM (USGS site ID `USGS-08330000`)
- **Parameter:** Discharge (`00060`), units in cubic feet per second (cfs)
- **Statistic:** Daily mean (`00003`)
- **Time period:** YYYY-MM-DD 
- **Outputs:**
  - Daily values stored in a pandas DataFrame and exported to a CSV file.
  - Monthly summary table (min, max, mean, total discharge) with parameter and statistic IDs.
  - Interactive Plotly time series with annual min/max reference lines.

## How to run the script
1. Install dependencies:
  ```bash
  pip install pandas requests plotly
  ```
2. Open the notebook and run all cells:
  - `daily_water_summary.ipynb`

## One thing you would improve with more time
Expand the workflow to pull data for all Rio Grande locations within New Mexico and analyze trends across the last five years.

