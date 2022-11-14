# Tree planning

J.D. Hamelink & T.C.J. Blom

## Setup

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Data

### Sources

[1] Trees: [NYC OpenData: _2015 Street Tree Census - Tree Data_](https://data.cityofnewyork.us/Environment/2015-Street-Tree-Census-Tree-Data/uvpi-gqnh)

[2] Traffic: [NYC OpenData: _Automated Traffic Volume Counts_](https://data.cityofnewyork.us/Transportation/Automated-Traffic-Volume-Counts/7ym2-wayt)

[3] Roads: [NYC OpenData: _NYC Street Centerline (CSCL)_](https://data.cityofnewyork.us/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b)


### Structure

The data directory should look like this:

```bash
data
├── csv
│   ├── 2015_Street_Tree_Census_-_Tree_Data.csv                   [1]
│   └── Automated_Traffic_Volume_Counts.csv                       [2]
├── shapefiles
│   └── NYC Street Centerline (CSCL)                              [3]
│       ├── geo_export_f4098162-199c-4100-9c2a-6bc6e35f8734.dbf
│       ├── geo_export_f4098162-199c-4100-9c2a-6bc6e35f8734.prj
│       ├── geo_export_f4098162-199c-4100-9c2a-6bc6e35f8734.shp
│       └── geo_export_f4098162-199c-4100-9c2a-6bc6e35f8734.shx
└── streets.geojson
```
