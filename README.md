# Easy Correlations

Easy Correlations is a forex trading strategy that uses Pearson correlation and RSI indicators to identify potential trading opportunities. This code provides an implementation of the Easy Correlations strategy in MQL4.

## Input Parameters

- Symbol1: The first currency pair to be considered for correlation analysis (default: 'EURUSD').
- Symbol2: The second currency pair to be considered for correlation analysis (default: 'GBPUSD').
- CorrelationPeriod: The period over which the correlation is calculated (default: 14).
- RsiPeriod: The period over which the RSI indicator is calculated (default: 14).
- RsiOverboughtLevel: The overbought level for the RSI indicator (default: 70.0).
- RsiOversoldLevel: The oversold level for the RSI indicator (default: 30.0).

## Global Variables

- correlation: Stores the calculated Pearson correlation value.
- rsi1: Stores the calculated RSI value for Symbol1.
- rsi2: Stores the calculated RSI value for Symbol2.
- previousCorrelation: Stores the previous correlation value.

## Custom Indicator Initialization

The OnInit() function is called when the indicator is initialized. In this function, the indicator plots three lines on the chart: the correlation line, and the RSI lines for Symbol1 and Symbol2. The indicator parameters are also set in this function.

## Custom Indicator Iteration

The OnCalculate() function is called for each new tick or bar. In this function, the correlation between Symbol1 and Symbol2 is calculated using the iCorrelation() function. The RSI values for Symbol1 and Symbol2 are calculated using the iRSI() function.

After calculating the correlation and RSI values, the code checks for divergence between the correlation and RSI values. If a divergence is detected, the code executes the trading rules specified in the comments. The trading rules involve buying Symbol1 and selling Symbol2, and placing stop loss and take profit levels.

The previous correlation value is updated at the end of the function.

## Product Description

Easy Correlations is a forex trading strategy that simplifies the process of identifying potential trading opportunities. It uses the correlation between two currency pairs and the RSI indicator to identify divergences that may indicate trading signals.

The strategy is implemented in this code, which provides an example of how the Easy Correlations strategy can be coded in MQL4. This code is not developed by ForexRobotEasy, but it serves as a reference for understanding how the strategy works.

To find the official developer of this product and for detailed reviews and trading results, please visit the following link: [Easy Correlations Review - Simplifying Forex Trading Strategy](https://forexroboteasy.com/forex-robot-review/easy-correlations-review-simplifying-forex-trading-strategy/)

Please note that ForexRobotEasy is not the official developer of this product.
