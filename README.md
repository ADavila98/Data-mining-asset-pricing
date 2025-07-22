**Stock Anomaly Analysis with WRDS Data in R**
**Overview**
This R script connects to the Wharton Research Data Services (WRDS) database, retrieves stock market (CRSP) and financial statement (Compustat) data, and performs analysis on common stock anomalies: Profitability, Size, and Value. It then merges these data with Fama-French 5-factor monthly data and calculates cumulative returns for each anomaly strategy within the manufacturing sector.

**Key Features**
Connects securely to WRDS using RPostgres

Retrieves and processes CRSP daily stock returns and Compustat firm fundamentals

Calculates anomaly metrics:

Profitability (ROA)

Size (market capitalization proxy)

Value (book-to-market ratio)

Applies winsorization to reduce outlier effects

Downloads and integrates Fama-French 5-factor data

Creates long-short anomaly strategies and computes cumulative returns

Visualizes strategy performance over time using ggplot2

Computes summary statistics (mean return, volatility, Sharpe ratio) for each strategy

**Dependencies**
DBI

RPostgres

dplyr, tidyr, tidyverse

DescTools

lubridate

ggplot2

tidyfinance

RSQLite

**Usage**
Replace @user@ and @password@ with your WRDS credentials.

Run the script to:

Connect to WRDS

Fetch and process data

Perform anomaly analysis

Generate plots and summary statistics
