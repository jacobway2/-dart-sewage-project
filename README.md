# Storm Overflows in the South West: A Three-Scale Analysis of Sewage Spills on the Dart, the South West, and England

A data-driven analysis of storm overflow spill counts on the River Dart, across the South West Water region, and nationally across English water companies, using Environment Agency and Met Office data from 2021 to 2024.

The full narrative writeup is available at: https://hackmd.io/@nXsN6esuSfCxk-psINDUjQ/HkBMdgMCbg

A copy paste of the narrative is also available in this repository as `blog_narrative.txt` incase the link above is inaccessible.

## How to Replicate

Clone the repository and navigate to the project folder, then install dependencies:

```
pip install -r requirements.txt
```

Then open and run the notebook from top to bottom in a fresh kernel:

```
jupyter notebook blog.ipynb
```

All data is fetched programmatically within the notebook. No manual downloads are required.

## Directory Structure

The project root contains blog.ipynb, README.md, requirements.txt, and blog_narrative.txt.

data/raw/ contains the four years of EDM Excel files downloaded from the EA, six Met Office regional rainfall text files, and twenty per-catchment gauge CSV files fetched from the EA Hydrology API.

data/processed/ contains five cleaned CSV files produced by the notebook: dart_overflows.csv, dart_rainfall_daily.csv, dart_annual_storm_days.csv, sww_rivers.csv, and national_summary.csv.

outputs/ contains all chart outputs produced by the notebook: seven PNG files used in the narrative, five additional PNG files produced for transparency and interactive exploration within the notebook, and the interactive folium map as folium_map.html.

## Data Sources & References

Environment Agency. (n.d.-a). Event Duration Monitoring - Storm Overflows - Annual Returns. www.data.gov.uk. Retrieved May 7, 2026, from https://www.data.gov.uk/dataset/19f6064d-7356-466f-844e-d20ea10ae9fd/event-duration-monitoring-storm-overflows-annual-returns

Environment Agency. (n.d.-b). Hydrology Data Explorer. environment.data.gov.uk. Retrieved May 7, 2026, from https://environment.data.gov.uk/hydrology/explore

Environment Agency. (n.d.-c). Catchment Data Explorer. environment.data.gov.uk. Retrieved May 7, 2026, from https://environment.data.gov.uk/catchment-planning/

Met Office. (2024). UK and Regional Series. Met Office. https://www.metoffice.gov.uk/research/climate/maps-and-data/uk-and-regional-series