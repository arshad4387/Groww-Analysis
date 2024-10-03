# Groww-Analysis

Problem Statement:
  Analyzing the stock trading data from Groww to identify top-performing and underperforming stocks across different trade types (Intraday, Short Term, Long Term) and also to view the P&L for each stock. 
  Aiming to provide better insights for better trading strategies.

Project Objective:
  Groww provides a detailed report containing all the transactions that we have made. Even though detailed reports are good to have, it's difficult to understand the metrics (profit & loss) on stock level. So, the objective is to create a summary of the existing report on stock level and to develop a comprehensive analysis framework that identifies the top 3 stocks that has the most gains and losses for each type of trade.

Data Description:
  Stock: The name of the stock.
  ISIN: International Securities Identification Number.
  Quantity: Number of shares traded.
  Buy Date: Date when the stock was purchased.
  Buy Price: Price at which the stock was bought.
  Buy Value: Total value spent on buying the stock.
  Sell Date: Date when the stock was sold.
  Sell Price: Price at which the stock was sold.
  Sell Value: Total value received from selling the stock.
  P&L: Profit and Loss from the trade.
  Remarks: Additional notes or comments on the trade.

Data Pre-processing Steps:
  Data Cleaning:
    Since we are using the report from Groww, data cleaning steps are very minimal.
    * Convert data types to appropriate formats (e.g., numeric types for stock quantity, buy value, sell value etc.)
  Grouping and Aggregating:
    Group by stock and trade type to summarize total values and P&L.

Assumptions:
  * The import file should be report exported from GROWW.
  * 
  * All trades are executed at the recorded prices and quantities.
  * The dataset accurately reflects all relevant trading activities and prices.
  * There are no transaction costs affecting the P&L values.

Model Evaluations and Techniques:
**Grouping** and Aggregating: Using pandas groupby to summarize data.

Ranking: Finding top and bottom performing stocks using pandas' nlargest and nsmallest functions.

Filtering: Ensuring only positive gains and negative losses are included in the respective summaries.

















