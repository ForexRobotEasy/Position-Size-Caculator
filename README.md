# Position Size Calculator

This code is a custom indicator for position size calculation in trading. It calculates the lot size and stop loss level based on the risk percentage and risk-reward ratio set by the user. The indicator also provides options to customize the entry level and place a horizontal line at the stop loss level.

## How it works

1. The indicator initializes by setting the necessary indicator properties and buffers.

2. In the `OnCalculate` function, the entry level is customized if the `CustomizeEntryLevel` option is enabled.

3. The account balance is retrieved using `AccountBalance()`.

4. The account risk is calculated by multiplying the balance with the risk percentage set by the user.

5. The reward is calculated by multiplying the account risk with the risk-reward ratio.

6. The entry price is set as the current close price.

7. The stop loss level is calculated by subtracting the reward from the entry price.

8. If the `PlaceStopLossLine` option is enabled, a horizontal line is created at the stop loss level.

9. The lot size is calculated by dividing the account risk by the difference between the stop loss and entry price.

10. The calculated lot size is returned.

## Product Description

**Position Size Calculator** is a powerful tool designed to simplify forex risk management. With this custom indicator, traders can easily calculate the appropriate lot size and determine the stop loss level based on their desired risk percentage and risk-reward ratio.

By inputting the risk percentage and risk-reward ratio, traders can quickly determine the lot size that aligns with their risk tolerance and trading strategy. The indicator also provides an option to customize the entry level, allowing traders to fine-tune their position entry.

Additionally, traders have the option to visualize the stop loss level by placing a horizontal line on the chart. This helps in monitoring the trade and making timely adjustments if needed.

To use this indicator effectively, simply attach it to your trading chart in MetaTrader platform and adjust the input parameters according to your risk management preferences. The indicator will automatically calculate and display the lot size and stop loss level.

Please note that ForexRobotEasy is not the official developer of this product. We are providing this sample code to demonstrate how the position size calculation can be implemented. For detailed reviews and trading results of the official product, please visit the official developer's website at [https://forexroboteasy.com/forex-robot-review/position-size-calculator-review-simplify-forex-risk-management/](https://forexroboteasy.com/forex-robot-review/position-size-calculator-review-simplify-forex-risk-management/). To find the official developer of this product, please refer to MQL5.
