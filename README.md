# Volume Momentum Analysis

## Project Details

### 1. Strategy Basic Idea

Objective: Analysis to find a tradeable pattern in volume surge, which could be used as an indicator to enter a trade in BUY/SELL direction. 

### 2. Kline Data File

BTC/USDT 5-min OHLCV (Open/High/Low/Close/Volume) data from Nov 2022 till May 2023.

* btc_ohlcv_5m.csv

#### Data Columns:

* market: "USDM" for all rows
* symbol: "BTC/USDT" for all rows
* unix: unix timestamp (in milliseconds) for start time of the bar
* open
* high
* low
* close
* volume

### 3. Strategy Specs

Customisable fields:

#### Entry-related:

* Signal condition: e.g. min volume threshold, etc
* Trade Side
* ...

#### Exit-related (for trade performance review):

* Take-profit level
* Cut-loss level
* ...

e.g. volume surge at bar_0 -> entry at bar_0 close (with TP at entry * (1 + m%); CL at entry * (1 - n%))
