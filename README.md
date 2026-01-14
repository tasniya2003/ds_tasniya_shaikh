# Market Sentiment vs Trader Performance

Google Colab Notebook:
https://colab.research.google.com/drive/1TjM4Ky60EKy7pswbXWGx7O_Y4RQLD21O?usp=sharing
This project analyzes the relationship between Bitcoin market sentiment and trader behavior using two datasets:
- Hyperliquid Historical Trading Data
- Bitcoin Fear & Greed Index
The goal is to understand how trader profitability, risk, and trading volume change under different market sentiment conditions (Fear, Greed, Neutral, Extreme Greed).

Folder Structure
ds_tasniya_shaikh/
├── notebook_1.ipynb
├── csv_files/ 
│   ├── historical_data.csv
│   ├── fear_greed_index.csv
│   ├── merged_data.csv
│   └── daily_trader_metrics.csv
├── outputs/
│   ├── pnl_by_sentiment.png
│   ├── volume_by_sentiment.png
│   └── leverage_by_sentiment.png
├── ds_report.pdf
└── README.md

Dataset Description
1. Hyperliquid Trading Data
- Contains real trading records including:
- Trader account
- Trade size in USD
- Buy/Sell direction
- Execution time
- Closed profit or loss (PnL)

2. Fear & Greed Index
- Provides daily market sentiment for Bitcoin based on volatility, volume, and momentum.
- Each day is classified as Fear, Greed, Neutral, or Extreme Greed.

Methodology
- Both datasets were loaded and cleaned in Google Colab.
- UNIX timestamps were converted into daily dates.
- Trading data was merged with the Fear–Greed Index using the trade date.
- Daily trader performance metrics were calculated.
- Visual analysis was performed to compare trading behavior across different sentiment states.

Outputs
- merged_data.csv – Trade-level data combined with sentiment
- daily_trader_metrics.csv – Aggregated daily performance

Charts in outputs/ show:
- Profit vs Sentiment
- Trading Volume vs Sentiment
- Average Trade Size (Risk) vs Sentiment

The key findings and interpretations are documented in ds_report.pdf.

How to Run
- Open notebook_1.ipynb in Google Colab and run all cells in order.
- All required CSV files are located in the csv_files folder.
