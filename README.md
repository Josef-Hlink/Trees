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
│   └── ny_traffic.csv
├── shapefiles
│   ├── ALTSTREETNAME_TBL.CPG
│   ├── ALTSTREETNAME_TBL.dbf
│   ├── ALTSTREETNAME_TBL.dbf.xml
│   ├── StreetSegment.CPG
│   ├── StreetSegment.dbf
│   ├── StreetSegment.prj
│   ├── StreetSegment.sbn
│   ├── StreetSegment.sbx
│   ├── StreetSegment.shp
│   ├── StreetSegment.shp.xml
│   └── StreetSegment.shx
└── streets.geojson
```

## Credentials (probably deprecated)

Credentials for the Foursquare API should be stored in a file called "credentials.json" in the root directory.
The file should contain the following:

```json
{
    "foursquare": {
        "client_id": "your-client-id",
        "client_secret": "your-client-secret",
        "authorization": "your-authorization"
    }
}
```
