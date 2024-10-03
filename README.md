# Groww-Analysis

## Table of Contents
1. [Introduction/Problem Statement](#introduction)
2. [Project Objective](#project-objective)
3. [Data Description](#data-description)
4. [Data Pre-processing](#data-pre-processing)
5. [Analysis](#analysis)
6. [Inspiration](#inspiration)
7. [Assumptions](#assumptions)
8. [Model Evaluations and Techniques](#model-evaluations-and-techniques)
9. [Inferences](#inferences)
10. [Future Possibilities](#future-possibilities)
11. [Conclusion](#conclusion)
12. [References](#references)
13. [Arshad](#summa)


## Introduction
  Analyzing the stock trading data from Groww to identify top-performing and underperforming stocks across different trade types (Intraday, Short Term, Long Term) and also to view the P&L for each stock, aiming to provide better insights for better trading strategies.

## Project Objective
  Groww provides a detailed report containing all the transactions that we have made. Even though detailed reports are good to have, it's difficult to understand the metrics (profit & loss) on stock level. So, the objective is to create a summary of the existing report on stock level and to develop a comprehensive analysis framework that identifies the top 3 stocks that has the most gains and losses for each type of trade.

## Data Description
  * _Stock_: The name of the stock.
  * _ISIN_: International Securities Identification Number.
  * _Quantity_: Number of shares traded.
  * _Buy Date_: Date when the stock was purchased.
  * _Buy Price_: Price at which the stock was bought.
  * _Buy Value_: Total value spent on buying the stock.
  * _Sell Date_: Date when the stock was sold.
  * _Sell Price_: Price at which the stock was sold.
  * _Sell Value_: Total value received from selling the stock.
  * _P&L_: Profit and Loss from the trade.
  * _Remarks_: Additional notes or comments on the trade.

## Data Pre-processing Steps
  * _Data Cleaning_:
    Since we are using the report from Groww, data cleaning steps are very minimal.
    * Convert data types to appropriate formats (e.g., numeric types for stock quantity, buy value, sell value etc.)
  * _Grouping and Aggregating_:
    Group by stock and trade type to summarize total values and P&L.
## summa
## Assumptions
  * The import file should be the report exported from GROWW.
  * All trades prices available in the report will be true as of buying/selling date.
  * The dataset accurately reflects all relevant trading activities and prices.

## Model Evaluations and Techniques
  * _Grouping and Aggregating_: Using pandas groupby to summarize data.
  * _Ranking_: Finding top and bottom performing stocks using pandas' nlargest and nsmallest functions.
  * _Filtering_: Ensuring only positive gains and negative losses are included in the respective summaries.
  * _Visualization_: Using IPython display the DataFrames together.

## Inferences
  * Helps to understand which stocks and trade types are performing well and which are not.
  * Easily identify top gains and top loss for each trade type.
  * Understand the platform charges, brokerage and DP charges.

## Future Possibilities
  * Fetching current data of the stocks from a database or using API's.
  * Incorporating machine learning models to predict future performance based on historical data.

## Conclusion
  This project provides a robust framework for analyzing stock trading performance, helping traders and investors make informed decisions. By identifying the top gainers and losers, one can refine trading strategies and improve profitability.
