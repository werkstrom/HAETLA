# HAETLA - High Automation ETL Architecture
A general purpose framework and tool for describing how to translate data from a bespoke structure to a general purpose Snowflake Schema Structure. The main feature is the ability to automatically adjust itself to changes in the source's structures. This is extremely useful when dealing with source's with datamodels that extend over time. Typically ERP systems and alike.

## Basic architecture
The framework consists of 
- Data Desciption Files. JSONC-files that describes how to transform the bespoke data
- Data Engine. Code that fetches raw data, translates it and saves it to a standardized Snowflake Schema
