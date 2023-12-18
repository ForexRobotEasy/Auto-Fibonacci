# Auto Fibonacci - Trading Robot

This code is a trading robot that uses the Fibonacci levels to determine entry points for buying trades. It is designed to be used with the MQL5 trading platform.

## How it Works

1. The code includes the necessary libraries for trading and calculating Fibonacci levels.

2. Global variables are defined to specify the stop loss, take profit, number of entry points to consider, and a unique identifier for the trades.

3. The code creates a trade object using the CTrade class.

4. The OnInit() function is called during the initialization of the code. In this function, the deviation in pips for trade execution is set.

5. The OnStart() function is called when the code starts running. In this function, the current market price is obtained using the SymbolInfoDouble() function.

6. Fibonacci levels are calculated using the CalculateFibonacciLevels() function, which takes the current price, an array to store the levels, and the number of entry points as parameters.

7. The code checks if there are enough entry points specified. If not, it prints an error message and stops execution.

8. The code loops through each entry point and checks if the current price is below the Fibonacci level. If it is, a buy trade is opened.

9. The position size is calculated based on the risk-to-reward ratio, which is the take profit divided by the stop loss. The position size is calculated using the AccountFreeMargin() function.

10. The trade.Buy() function is called to open a buy trade with the calculated position size, stop loss, take profit, and the unique identifier.

11. Trade information is printed, including the price at which the trade was opened, the stop loss, and the take profit.

12. The loop is exited after the first entry point that satisfies the condition is found.

13. The OnDeinit() function is called during deinitialization of the code. In this function, any open trades are closed using the trade.CloseAll() function.

## Product Description

This code is a sample trading robot that uses Fibonacci levels to determine entry points for buying trades. It is designed to be used with the MQL5 trading platform. 

The Auto Fibonacci - Trading Robot is an automated trading system that can help traders identify potential entry points based on Fibonacci levels. Fibonacci levels are widely used in technical analysis and are believed to provide support and resistance levels in financial markets.

With this trading robot, traders can set their desired stop loss and take profit levels, as well as specify the number of entry points to consider. The robot will then calculate the Fibonacci levels based on the current market price and open a buy trade if the price is below any of the calculated levels.

The position size is automatically calculated based on the risk-to-reward ratio, which allows traders to manage their risk effectively. The robot also provides trade information, including the price at which the trade was opened, the stop loss, and the take profit.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in this product. To find the official developer of this product, please refer to MQL5. 

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Auto Fibonacci Forex Software Review and Real Results](https://forexroboteasy.com/forex-robot-review/auto-fibonacci-forex-software-review-and-real-results/).
