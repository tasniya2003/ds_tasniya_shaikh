# Market Sentiment vs Trader Performance

Google Colab Notebook:
https://colab.research.google.com/drive/1TjM4Ky60EKy7pswbXWGx7O_Y4RQLD21O?usp=sharing
Datasets Used
1. Hyperliquid Historical Trading Data
This dataset contains real trading records, including:
- Trader account ID
- Trade size in USD
- Buy/Sell direction
- Execution timestamp
- Closed profit or loss (PnL)

2. Bitcoin Fear & Greed Index
This dataset provides daily Bitcoin market sentiment based on:
- Market volatility
- Trading volume
- Price momentum
Each day is classified as Fear, Greed, or Neutral.

Methodology
- Both datasets were loaded and cleaned using Google Colab.
- UNIX timestamps were converted into daily dates.
- Trading data was merged with the Fear–Greed Index using the trade date.
- Daily trader-level performance metrics were calculated.
- Visual analysis was performed to compare trader performance and risk behavior across sentiment states.

Outputs
- The project generates the following outputs:
- merged_data.csv – Trade-level data combined with market sentiment
- daily_trader_metrics.csv – Aggregated daily trader performance metrics
The outputs/ folder contains:
- pnl_by_sentiment.png – Average daily PnL by market sentiment
- leverage_by_sentiment.png – Average trade size by market sentiment

Key findings and interpretations are summarized in ds_report.pdf.

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
│   └── leverage_by_sentiment.png
├── ds_report.pdf
└── README.md
