# CFTC
Each Friday the CFTC publishes its Commitment of Traders reports showing long and short positions in financial and commodity futures as of that Tuesday.
This is the scraper for all the data published by CFTC, including:
* Disaggregated Futures Only Reports
* Disaggregated Futures-and-Options Combined Reports
* Traders in Financial Futures; Futures Only Reports
* Traders in Financial Futures; Futures-and-Options Combined Reports
* Futures Only Reports
* Futures-and-Options Combined Reports
* Commodity Index Trader Supplement


## config
PostgreSQL DB setting

## config/config.yml
SQL Server DB setting

## sql
the table create command for all the CFTC data (PostgreSQL)

## sql_sqlserver
the table create command for all the CFTC data (SQL Server)

## data
(PostgreSQL)
if the table doesn't exist, this script will create for you
run the script each Friday after CFTC publishes the reports to update the data

## data_sqlserver
(SQL Server)
if the table doesn't exist, this script will create for you
run the script each Friday after CFTC publishes the reports to update the data
* Using pytds for performance
* All datalayer code are located in datalayer_sqlserver.py

![image](https://user-images.githubusercontent.com/4289161/156403826-7ec48f7c-5704-4446-89f1-cec77f9fb76b.png)

## historical_data\daily_data

Several futures daily data.

![image](https://user-images.githubusercontent.com/4289161/176221898-2a4f9ad2-bca0-4df2-b89f-229a6ddea73c.png)

## jack_seasonal_trading_strategy_back_test

* daily_data_to_sql_server.ipynb
Insert data into SQL Server.





