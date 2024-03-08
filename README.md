# SwingTradePro2

SwingTradePro2 is an Expert Advisor (EA) developed by Forex Robot Easy that trades the Forex market using a trend-searching algorithm based on three moving averages. The EA enters long trades when the price is above the moving average (MA) and the second MA crosses the third MA from bottom to top. It enters short trades when the price is below the MA and the second MA crosses the third MA from top to bottom. The EA also allows flexible settings for stop loss and take profit, and provides an option to close trades following a counter signal.

## Installation

To use SwingTradePro2, follow these steps:

1. Download and install the MetaTrader 5 platform from [MQL5](https://www.mql5.com/en/metatrader5).
2. Open MetaEditor in MetaTrader 5.
3. Create a new Expert Advisor.
4. Copy and paste the code provided into the Expert Advisor file.
5. Save the Expert Advisor file.
6. Compile the Expert Advisor.
7. Attach the Expert Advisor to a chart in MetaTrader 5.

## Settings

The EA has the following global variables that can be modified:

- `StopLoss` (integer): The default stop loss in points.
- `TakeProfit` (integer): The default take profit in points.
- `RiskRewardRatio` (double): The default risk reward ratio.
- `CloseOnCounterSignal` (boolean): Whether to close trades following a counter signal.

## How it Works

The Expert Advisor uses the `OnInit()` function for initialization. In this function, the stop loss and take profit levels are set based on the risk reward ratio. The initial settings are then printed.

The `OnTick()` function is called on each tick of the price. In this function, the EA checks if the conditions for a long trade or a short trade are met. If so, it places the corresponding trade using the `OrderSend()` function.

If the close on counter signal option is enabled, the EA checks if a counter signal is detected. If so, it closes the existing trades using the `OrderClose()` function.

The `OnDeinit()` function is used for any necessary cleanup.

## Product Description

SwingTradePro2 is an advanced Expert Advisor designed to trade the Forex market with high efficiency. Developed by Forex Robot Easy, this EA utilizes a trend-searching algorithm based on three moving averages to identify profitable trading opportunities.

With SwingTradePro2, you can take advantage of long trades when the price is above the moving average and the second moving average crosses the third moving average from bottom to top. Similarly, short trades are executed when the price is below the moving average and the second moving average crosses the third moving average from top to bottom.

One of the key features of SwingTradePro2 is its flexibility in settings. You can easily adjust the stop loss and take profit levels according to your risk appetite. Additionally, the EA provides an option to close trades following a counter signal, allowing you to exit positions if a change in market direction is detected.

To ensure transparency and reliability, we have provided a sample code for SwingTradePro2. Please note that Forex Robot Easy is not the official developer of this product. We recommend visiting the official MQL5 website to find the official developer and access detailed reviews and trading results of SwingTradePro2.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/swing-trade-pro-2-mt5-review-automated-forex-trading-efficiency/).

Note: The code provided is a sample and may require customization or further development to suit your specific trading needs.
