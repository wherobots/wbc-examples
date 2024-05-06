# Wherobots Open Data Examples

This repository contains examples notebooks for Wherobots Cloud Open
Data. These notebooks only work on [Wherobots Cloud](https://cloud.wherobots.com),
and use datasets only available to Wherobots Professional Edition users.

*Insurance Risk Analysis Use Case*

<img src="images/wbc-use-case-insurance.gif" width="800">

*Fleet Traffic Analysis Use Case*

<img src="images/wbc-use-case-fleet.gif" width="800">

*Aircraft Flight Analysis Use Case*

<img src="images/wbc-use-case-flights.gif" width="800">

## Wherobots open data

Wherobots offers two open data catalogs:

* `wherobots_open_data`, accessible to all Wherobots Cloud users;
* `wherobots_pro_data`, only available to Professional Edition users.

All data in those catalogs is stored in SedonaDB's Havasu table format.
More information about Wherobots' open data catalogs is available on the
[Wherobots documentation
website](https://docs.wherobots.com/latest/tutorials/opendata/introduction/).

```sql
SHOW SCHEMAS IN wherobots_pro_data

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

To become a Professional Edition user, please [contact us](https://wherobots.com/contact).

## Repository structure

The structure of this repository is as follows:

* `python/`: Python notebooks
	* `data-source/`: example notebooks for loading and saving data from/to Snowflake and AWS RDS PostGIS
	* `use-cases/`: use case examples for analyzing data using Wherobots Open data
* `scala/`: Scala notebooks
	* `data-source/`: example notebooks for loading and saving data from/to Snowflake and AWS RDS PostGIS

We recommend to use at least a "San Francisco"-sized Sedona runtime to
run those example use-cases (24 total cores, 96GB total memory).

## Data source notebooks

Data source notebooks require you to enter your own Snowflake / PostGIS credentials.
