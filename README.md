# Transit_ETL
----

This repository was part of a project which takes in logs of **~17 TB** (compressed as .gz) [nd json](http://ndjson.org/) (stored in AWS S3) and creates a mysql warehouse using the schema defined in the [database.sql](database.sql) file.
All ETL work was nodejs, and currently in the process of converting it with python.


### Getting started
----

- Install NodeJS (https://nodejs.org/en/)
- Inside the script folder, run the command `npm install`
- Change the MySQL connection configuration in worker.js
- run `DEBUG=* nodejs ./query.sh process ./data/ 20160502 1` where `session-20160502.gz` is the file in the data folder `1` represents number of file you want to process


![](TransitApp_Table May 2015_schema.png?raw=true "Schema")
