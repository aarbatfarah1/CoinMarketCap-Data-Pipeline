# Cryptocurrency Data Pipeline with DBT and CoinMarketCap API

## Project Overview
This project demonstrates an end-to-end data pipeline using data from the CoinMarketCap API, PostgreSQL for data storage, DBT for data transformations, and Power BI for visualization.

## Pipeline Workflow
1. **Extract**: Fetch the top 100 cryptocurrencies by market cap from the CoinMarketCap API.
2. **Load**: Store the raw data in PostgreSQL's `staging` schema.
3. **Transform**: Use DBT to clean, transform, and load the data into the `prod` schema.
4. **Visualize**: Connect Power BI to PostgreSQL for data visualization.

## Project Diagram
![Project Diagram](Project%20Diagram/Project%20Diagram.png)


## Setup Instructions
1. Clone this repository.
2. Create an account on [CoinMarketCap API](https://coinmarketcap.com/api/) and obtain an API key.
3. Set up a PostgreSQL database with `staging` and `prod` schemas.
4. Configure DBT:
   - Install DBT (`pip install dbt`).
   - Initialize a DBT project (`dbt init <project_name>`).
   - Update `profiles.yml` with your PostgreSQL connection details.
5. Run the pipeline:
   - Fetch data from CoinMarketCap API using the provided Python script.
   - Load the data into PostgreSQL.
   - Run DBT models (`dbt run`) to transform the data.
6. Connect Power BI to PostgreSQL and visualize the data.

## Requirements
- Python
- PostgreSQL
- DBT
- Power BI (or any preferred visualization tool)

## The final output
![PowerBI Dashboard](PowerBI%20Dashboard/PowerBI%20Dashboard.png)

