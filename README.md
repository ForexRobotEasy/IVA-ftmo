# IVA FTMO - Chart Setup

This code is a part of the IVA FTMO Forex trading robot developed by Forex Robot Easy. This code sets up the chart for trading by opening a chart with a specified symbol and period, and configuring various chart properties such as foreground color, grid, and scale.

## Global Variables
- `g_symbolIndex`: A global variable used to keep track of the current symbol index.

## Chart Setup Function
The `ChartSetup()` function is responsible for setting up the chart for trading. It performs the following tasks:
1. Sets the symbol based on the symbol index.
2. Opens the chart with the specified symbol and period.
3. Sets the chart properties such as foreground color, grid, and scale.

## Trading Logic

The `TradingLogic()` function contains the main trading algorithm for the IVA FTMO robot, which is based on a grid system. It implements entry and exit conditions, entry price calculation, stop loss calculation, trade execution, and trade closure.

### Entry Condition Check Function
The `IsGridEntryConditionMet()` function checks if the entry condition for the grid system is met. It implements the entry condition logic based on the grid system and returns true if the entry condition is met, otherwise false.

### Get Entry Price Function
The `GetEntryPrice()` function calculates the entry price based on the implemented logic and returns the calculated entry price.

### Calculate Stop Loss Function
The `CalculateStopLoss()` function calculates the stop loss based on the entry price and returns the calculated stop loss.

### Execute Trade Function
The `ExecuteTrade()` function executes the trade at the entry price with the calculated stop loss.

### Exit Condition Check Function
The `IsGridExitConditionMet()` function checks if the exit condition for the grid system is met. It implements the exit condition logic based on the grid system and returns true if the exit condition is met, otherwise false.

### Close Trade Function
The `CloseTrade()` function closes the current trade.

## Currency Pair Support

The `CurrencyPairSupport()` function sets up multiple charts with different currency pairs. It loops through an array of currency pairs, opens a chart for each pair with the specified period, and sets the chart properties.

## Backtesting

The `Backtesting()` function performs backtesting for the IVA FTMO robot. It sets the backtesting parameters such as start date and end date, and then iterates through each time period to simulate trading. For each time period, it sets the current time, and calls the `TradingLogic()` function to execute the trading logic.

## Main Program

The `OnStart()` function is the main program of the IVA FTMO robot. It calls the `ChartSetup()` function to set up the chart, the `CurrencyPairSupport()` function to set up multiple currency pair charts, and the `Backtesting()` function to perform backtesting.

Note: ForexRobotEasy is not the official developer of the IVA FTMO robot. This code is provided as a sample and may not fully represent the functionality of the official product. To find the official developer and obtain the complete and accurate version of this product, please refer to MQL5. For detailed reviews and trading results of this product, you can visit [ForexRobotEasy's IVA FTMO Review](https://forexroboteasy.com/forex-robot-review/iva-ftmo-review-advanced-grid-system-for-forex-trading/).
