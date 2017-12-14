# Grand Bahama Port Authority GIS Databases

Dec 2017

## Overview
This repo contains the full export of all the GIS data stored and managed by the Grand Bahama Port Authority (GBPA) regarding the **City of Freeport** and **Grand Bahama Island**. It includes points (lat/lon), shapes/envelopes, lines, and all other geographic/geometric data about Grand Bahama.

It is actively being curated and added to on a scheduled basis.

Since 2005 the department has been creating new data in the form of GIS Layers, as well as updating and maintaining existing ones. The Goal of the department is to create a seamless, rich, accurate data set of the Port Area to facilitate development and assist the licensees of the Port Area in their business.

In addition to GIS Services the department also maintains a digital archive of Survey Plans and Architectural documents. Copies of these documents may be obtained from our office at the Grand Bahama Medical Complex, or online using our form.

Our data is made freely available to vendors, developers, designers, planners, or analysts to use in applications, without restrictions.

**Official GIS site for Grand Bahama**:
https://gis.gbpa.com/

REST API to test against (no authentication required):
https://api.gis.gbpa.com

## Licensing
The data supplied in the repo is provided by the Grand Bahama Port Authority (GBPA) for third parties to use or modify under a **Creative Commons Attribution 4.0 International (CC BY 4.0)** license. Please include *"Data Provided by The Grand Bahama Port Authority"* in both the source code and UI of your application where possible.

**Important OSM Note**: The data may also be imported into OpenStreetMap under the ODbL 1.0 with no further need for formal permission (see: https://blog.openstreetmap.org/2017/03/17/use-of-cc-by-data/)

## Mapbox Datasets
All the files under 5MB are available to the Mapbox Community for use as tilesets in your applications. Our username when searching is **gbpa**.

Mapbox API link:
https://api.mapbox.com/datasets/v1/gpba

## Raw SQL Dump
You can find a ready-made .sql file of all 62,000 addresses in Freeport City in the `SQL/` folder which you can use to create a quick reference table in MySQL/Maria or other compatible RDBMS.

## Formats
**Important**: the most comprehensive collections are our GeoJSON datasets. Some of the formats do not feature complex shapes like MultiPolygons. The CSV data mainly contains listings of the records themselves, whereas the more modern formats contain the full shapes.

If you are in doubt as to where to start, try opening the ArcGIS shape files (.shp) in a desktop GUI like **qGIS** (https://www.qgis.org/en/site/). You can export the raw data yourself.

- **Esri ArcGIS**: how we store the data we collect (.shp files)
- **CSV:** raw data compatible with most languages, open in Excel
- **Geography ML**: older XML format for OpenGIS
- **GeoJSON**: mewest, for platforms like Google Maps API and Mapbox API
- **KML**: Keyhole ML (XML), used by Google Maps/Earth
- **SQL**: quick import into MySQL/Postgres
- **Spatialite**: spatial extension of SQLite portable DB file (useful for offline iOS/Android apps)
- **Well-Known Text**: for C-based libraries, and/or MySQL spatial/PostGIS

## Quick Start

If you need to get into the original data on your **desktop**, drag the .shp files into qGIS (https://www.qgis.org/en/site/).

If you need to show the data to non-technical users on a desktop, open the **KML** files with **Google Earth** (https://www.google.com/earth/).

If you are building a **web app**, use the **GeoJSON** files - easily stored in NoSQL databases, or as a JSON field in other RDBMS/Elasticsearch. View/test with http://geojson.io/.

If you are building an **iOS/Android app** and need offline map data, **zip** the files for inclusion into your bundle, or consider using the **Spatialite** (https://www.gaia-gis.it/fossil/libspatialite/index) standalone files.

## Further Information
Please contact:

GIS Department
Grand Bahama Port Authority Limited
Pioneers Way & East Mall Drive
P.O. Box F-42666
Freeport, Grand Bahama Island
Tel: 242-350-9000
Fax: 242-352-6184
