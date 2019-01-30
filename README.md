# curve-building
Libor curve bootstrapping example from cash, Eurodollar future and interest rate swap instruments.

The spreadsheet contains six tabs.

- BBG Replica
- BBG Data Table
- BBG Input
- BBG Input Tickers
- BBG Output
- BBG Output Tickers

On the "BBG Input" tab, one can see Bloomberg screen shots of the input data. Input tab screen shot has three instrument groups - Cash Rates, Contiguous Futures, and Swap Rates. Instruments that are used for bootstrapping are highlighted in orange. The Zero Rates Chart at the bottom is the output curve. This curve is broken into three segments - short end, middle, and long end. Notice, that Contiguous Futures quotes contain prices and convexity adjustments that can be converted into forward rates. The day counting conventions, maturity dates, and terms are also captured on this tab. We have recorded input data on the "BBG Data Table" tab. The data from this tab will be referenced on the main calculation tab, the "BBG Replica" tab.

On the "BBG Output" tab, one can see Bloomberg output - zero rates and discount factors. In our calculations, we will focus on the discount factors. Our calculated discount factors are compared to these Bloomberg output rates on the "BBG Replica" tab. Bloomberg tickers corresponding to the input and output rates are captured on the "BBT Input Tickers" and "BBG Output Tickers" tabs.

Finally, the discount factors are calculated on the "BBG Replica" tab. Rows corresponding to different instrument types are filled with different colors - red for cash, blue for EDF, and white for swap. Instrument specific discount factor formulas are captured at the bottom of this tab. The calculated discount factors are compared to the Bloomberg output in the last two columns. There is also a check on the swap value in rows 22-23, columns E-G. The value of the interest rate swap with fixed rate set to the spot swap rate should be 0.
