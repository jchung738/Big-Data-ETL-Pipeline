# Understanding User Behavior With ETL Pipeline

- The game has two events we're interested in tracking: `buy a
  sword` & `join guild`

- Each has metadata characterstic of such events (i.e., sword type, guild name,
  etc)


## Aspects of the Project

- Instrumented an API server in game_api.py to log events to Kafka

- Assembled a data pipeline to catch these events: using Spark streaming to filter
  select event types from Kafka, landing them into HDFS/parquet to make them
  available for analysis using Presto

- Used Apache Bench to generate test data for your pipeline

- Produced an analytics report where I provided a description of my pipeline
  and some basic analysis of the events

The iPython notebook includes both the CLI commands to set up the pipeline with 
descriptions of each command, and some basic analysis of the Apache Bench generated
user events.

Note: This pipeline was created within the Google Cloud platform.

