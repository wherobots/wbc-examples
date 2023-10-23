# Wherobots Open Data Examples

This repository contains examples notebooks for Wherobots Cloud Open Data. These notebooks only work on [Wherobots Cloud](https://wherobots.services).

<img src="images/wbc-use-case-insurance.gif" width="800">

<img src="images/wbc-use-case-fleet.gif" width="800">

## Wherobots open data

Wherobots open data catalog below is only accessible by the pro edition users. All data are preproccessed and stored in SedonaDB Havasu table format. Detailed description about Wherobots open data is available on [Wherobots documentation website](https://docs.wherobots.services/latest/tutorials/opendata/introduction/).

```
+----------------+
|       namespace|
+----------------+
|google_microsoft|
|         landsat|
|        nyc_taxi|
|             osm|
|       us_census|
|         weather|
+----------------+
```

To become a pro edition user, please [contact us](https://wherobots.ai).

## Repo structure

The structure of this repo is as follows:

* Python: Python notebooks
	* data-source: example notebooks for loading and saving data from/to Snowflake and AWS RDS PostGIS
	* use-cases: use case examples for analyzing data using Wherobots Open data
* Scala: Python notebooks
	* data-source: example notebooks for loading and saving data from/to Snowflake and AWS RDS PostGIS

We recommend to use a Sedona cluster with 40+ CPU cores and 100GB+ RAM for running the use case notebook.

## Data source notebooks

Data source notebooks require you to enter your own Snowflake / PostGIS credentials.
