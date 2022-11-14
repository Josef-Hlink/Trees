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

Traffic: [NYC OpenData: _Automated Traffic Volume Counts_](https://data.cityofnewyork.us/Transportation/Automated-Traffic-Volume-Counts/7ym2-wayt)

Trees: [NYC OpenData: _2015 Street Tree Census - Tree Data_](https://data.cityofnewyork.us/Environment/2015-Street-Tree-Census-Tree-Data/uvpi-gqnh).

You will notice that some sources are not listed.
This is due to us not being sure whether or not to actually use this data.

### Structure

This is my data directory structure as of now, but it will definitely change.

```bash
data
├── csv
│   ├── 2015_Street_Tree_Census_-_Tree_Data.csv
│   ├── Automated_Traffic_Volume_Counts.csv
│   └── sample_traffic.csv
├── shapefiles
│   └── NYC Street Centerline (CSCL)
│       ├── geo_export_f4098162-199c-4100-9c2a-6bc6e35f8734.dbf
│       ├── geo_export_f4098162-199c-4100-9c2a-6bc6e35f8734.prj
│       ├── geo_export_f4098162-199c-4100-9c2a-6bc6e35f8734.shp
│       └── geo_export_f4098162-199c-4100-9c2a-6bc6e35f8734.shx
└── streets.geojson
```
