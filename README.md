# OSM-RDF
Converting OSM administrative boundaries to RDF

##Requirements
NodeJS and JAVA

## Installation

- run `npm install`
- go to ./data folder

    - run `./downloadData` bash script to download all the required OSM shape files.
    - run `./installOSMOSIS` bash script to install OSMOSIS for processing OSM data.
    - run `./extractAdminBoundaries` bash script to process and extract administrative boundaries from the data.
    - run `./convertOSMtoGeoJSON` bash script to convert the extracted data to GeoJSON format.
    - run `geojson-rdf [level] [file_or_uri_to_convert]`

## Usage

`geojson-rdf [country_iso3] [file_or_uri_to_convert]`

Example:

`./geojson-rdf NLD netherlands.geojson`

 or

`./geojson-rdf AUTO netherlands.geojson`
for automatic detection of country name
