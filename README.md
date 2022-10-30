# Tree planning

J.D. Hamelink & T.C.J. Blom

## Usage

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
raster2xyz data/bomenkaart.tif data/csv/bomenkaart.csv
```

## Data

Data folder should contain "bomenkaart.tif" from [Nationaal Georegister](https://www.nationaalgeoregister.nl/geonetwork/srv/dut/catalog.search#/metadata/89611780-75d6-4163-935f-9bc0a738f7ca).

In the data directory, there should also be a "shapefiles" subdir with the contents of the "shapefiles.zip" file from [EarthWorks](https://earthworks.stanford.edu/catalog/stanford-gp502yc4422).

### Structure

This is my data directory structure as of now, but it will definitely change.

```bash
data
├── bomenkaart.tif
├── stikstofdepositie.gpkg
├── csv
│   ├── bomenkaart.csv
│   └── fsq_venues.csv
└── shp
    ├── ADM0
    ├── provincies
    └── restwarmte
```

## Credentials

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
