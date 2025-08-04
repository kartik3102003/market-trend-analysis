{\rtf1\ansi\ansicpg1252\cocoartf2822
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # \uc0\u55357 \u56520  Market Trend Analysis \'96 Commodity Futures\
\
This project simulates a simple trend-following strategy using historical price data of a commodity (Gold ETF - GLD). The goal was to analyze whether a moving average crossover system could yield profitable signals in commodity markets.\
\
---\
\
## \uc0\u55358 \u56800  Objective\
\
- Implement and evaluate a **moving average crossover strategy** (20-day vs 50-day SMA)\
- Simulate **buy/sell signals** based on trend direction\
- Measure hypothetical returns and analyze strategy behavior\
\
---\
\
## \uc0\u55357 \u57056 \u65039  Tools & Libraries\
\
- Python\
- Pandas\
- Matplotlib\
- yfinance (for fetching historical data)\
\
---\
\
## \uc0\u55357 \u56522  Strategy Details\
\
- **Asset**: Gold ETF (`GLD`)\
- **Time Period**: Jan 2020 \'96 Dec 2023\
- **Buy Signal**: 20-day SMA crosses above 50-day SMA\
- **Sell Signal**: 20-day SMA crosses below 50-day SMA\
- **Position**: +1 (long), -1 (short), shifted forward by 1 day\
- **Returns**: Based on percentage change \'d7 strategy position\
\
---\
\
## \uc0\u55357 \u56521  Outcome\
\
- **Hypothetical Strategy Return**: **-18.9%**\
- The strategy underperformed in this timeframe, indicating limitations in trend-following systems during volatile or sideways markets.\
- This highlights the need for adaptive techniques or additional filters such as volatility checks or stop-loss limits.\
\
---\
\
## \uc0\u55357 \u56520  Visualization\
\
The notebook includes a plotted chart showing:\
- Price of the commodity\
- 20-day and 50-day moving averages\
- Crossover points and price trends\
\
---\
\
## \uc0\u55357 \u56550  Getting Started\
\
### Installation:\
```bash\
pip install pandas matplotlib yfinance\
}