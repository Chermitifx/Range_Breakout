# Range_Breakout

Range Breakout Expert Advisor (EA) for MetaTrader5

Key Features:

Fixed Lot Size / Martingale Option:

   Fixed Lot Size:* The EA allows you to set a constant lot size for each trade.
   Martingale Option:* Alternatively, you can enable the Martingale strategy, which increases the lot size after a losing trade to recover losses.
Trading Between Specific Times:

    The EA only opens trades within a specified time range (e.g., 08:00 to 18:00). This helps avoid trading during low-liquidity periods.
Trading Days :

Take Profit and Stop Loss as Multipliers of the Range:

    The take profit (TP) and stop loss (SL) levels are calculated based on a multiplier of the range width (distance between support and resistance).
    For example, if the range is 50 pips and the multiplier is 2, the TP and SL would be 100 pips.
EMA Option to Detect Trend:
   The EA uses an Exponential Moving Average (EMA) to filter trades in the direction of the trend.
   Only trades in the direction of the EMA trend are taken (e.g., only long trades if the price is above the EMA).
Trailing Stop Loss:
   A trailing stop loss option is available to protect profits.
   The stop loss moves in the direction of the trade as the price moves favorably, locking in profits as the trade progresses.
How The EA +Works:

1. Identify the Range:
   The EA monitors the market to identify a price range with clear support and resistance levels.
2. Wait for a Breakout:
   The EA waits for the price to break above the resistance level or below the support level.
3. Check the Trend (if EMA is enabled):
   The EA checks the EMA to ensure the breakout is in the direction of the trend.
4. Place Trades:
   When a breakout is confirmed in the direction of the trend, the EA places a trade.
   The lot size is either fixed or adjusted according to the Martingale strategy.
5. Set TP and SL:
   The EA sets the take profit and stop loss based on the range multiplier.
6. Apply Trailing Stop Loss:
   As the trade moves in the favorable direction, the trailing stop loss adjusts to lock in profits.
Example Settings:

- Fixed Lot Size: 0.1 lots
- Martingale Multiplier: 2 (if enabled)
- Trading Time: 08:00 to 18:00
- Range Multiplier for TP/SL: 2
- EMA Period: 50
- Trailing Stop Loss: 20 pips

This EA helps automate the range breakout trading strategy, allowing traders to focus on other tasks while the EA manages trade entries, exits, and risk management based on the defined parameters.
