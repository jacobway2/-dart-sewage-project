# Sewage on the Dart: How Bad Is It Really, and How Does It Compare?

**BEE2041: Data Science for Economics — Empirical Project**

project analyses storm overflow (sewage discharge) data on the river dart>places it in 
the context of all South West Water rivers>then England as a whole>uses environment agency 
event duration monitoring (EDM) data>normalised against rainfall data>data from two environment
agency hydrology API gauges within the dart catchment (defined by the environment agencys 'catchment data explorer')>asks - is the dart particularly bad and how does it compare to others in the SWW region and the country as a whole?

---

## Repository Structure

```
dart-sewage-project/
├── README.md               ← this file
├── blog.ipynb              ← the notebook
├── data/
│   ├── raw/                ← files as downloaded
│   └── processed/          ← cleaned files produced by the notebook
└── outputs/                ← saved plot images
```

---

## Data Sources

### 1. Storm Overflow (EDM) Data
**Source:** Environment Agency Event Duration Monitoring Annual Returns  
**URL:** https://www.data.gov.uk/dataset/19f6064d-7356-466f-844e-d20ea10ae9fd/  
Annual Excel files (one per year, 2020–2024) containing spill counts and durations.

### 2. Rainfall Data
**Source:** Environment Agency Hydrology API  
**URL:** https://environment.data.gov.uk/hydrology/  
Daily rainfall readings from two gauges within the Dart catchment:
- Holne Priddacott Farm (Telemetry Ref 46169, WISKI ID 363710)
- Austins Bridge rainfall gauge (Telemetry Ref 46103, WISKI ID 364176)

No API key is required for either dataset.

---

## How to Reproduce

### 1. Clone the repository
git clone https://github.com/<username>/dart-sewage-project.git
cd dart-sewage-project

### 2. Install dependencies

pip install -r requirements.txt

### 3. Run the notebook
jupyter notebook blog.ipynb


Run all cells from top to bottom
The notebook will:
- Download all EDM Excel files
- add other stuff here later

---

## Dependencies

See `requirements.txt`