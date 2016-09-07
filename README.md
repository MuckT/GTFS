# GTFS

Public transportation schedules and associated geographic information for South-East Queensland.

The data is a snapshot and not planned to be kept up-to-date. The main purpose of this repository is to develop a data package for this dataset.

## Data
This data is the [General transit feed specification (GTFS) — South East Queensland](https://data.qld.gov.au/dataset/general-transit-feed-specification-gtfs-seq) data published by [Transport and Main Roads, Queensland Government](http://www.tmr.qld.gov.au/), licensed under [Creative Commons Attribution](https://creativecommons.org/licenses/by/3.0/au/) sourced on 07 September 2016.

The data is follows the [GTFS specification](https://developers.google.com/transit/gtfs/reference/) and some of its [extensions](https://developers.google.com/transit/gtfs/reference/gtfs-extensions) that define a common format for public transportation schedules and associated geographic information. The specification allows some files to be optional. It also allows some columns in the files to be optional. This means that the datapackage.json file and schemas may not work for [other GTFS files](https://code.google.com/archive/p/googletransitdatafeed/wikis/PublicFeeds.wiki).

[The data](https://github.com/Stephen-Gates/GTFS/tree/master/data) is made up of a number of files. Two data files (shapes.txt and trips.txt) were too large to load into GitHub. They were truncated. They will be adequate to use for testing valid data.

Each data file is defined by a [schema](https://github.com/Stephen-Gates/GTFS/tree/master/schemas). The schemas follow the [json table schema specification](http://specs.frictionlessdata.io/json-table-schema/)

These schemas are combined into a datapackage.json file to fully describe the data collection. The datapackage.json file follows the [specification](http://specs.frictionlessdata.io/data-packages/).

## Preparation
Put information on preparing the data in a Preparation section. In particular, any instructions about how to run any preparation and processing scripts to generate the data should go here.

## Tests
The data is tested using [GoodTables](http://goodtables.okfnlabs.org).
The data is then tested using GoodTables and the relevant schema.
Lastly the [test data](https://github.com/Stephen-Gates/GTFS/tree/master/tests) is used in GoodTables using the relevant schema to ensure the schema detects all errors (e.g. [incorrect types](http://specs.frictionlessdata.io/json-table-schema/#field-types-and-formats) and [constraints](http://specs.frictionlessdata.io/json-table-schema/#field-constraints))



## License
All items in this repository, apart from the data, are licenced under [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/).
