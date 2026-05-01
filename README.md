# Bitcoin Trader Performance vs Market Sentiment Analysis

## Overview
Analysis of **211,224 trades** from Hyperliquid DEX against the Bitcoin Fear & Greed Index to uncover how market sentiment impacts trader performance.

## Datasets
- `historical_data.csv` — Hyperliquid trader data (Dec 2023 – Apr 2025)
- `fear_greed_index.csv` — Daily Bitcoin Fear & Greed Index classifications

## Key Findings
| Sentiment | Total PnL | Avg PnL/Trade | Win Rate |
|-----------|-----------|---------------|----------|
| Extreme Fear | $739K | $35 | 76.2% |
| Fear | $3.36M | $54 | 87.3% |
| Neutral | $1.29M | $34 | 82.4% |
| Greed | $2.15M | $43 | 76.9% |
| Extreme Greed | $2.72M | $68 | 89.2% |

## Charts Generated
1. `chart1_pnl_by_sentiment.png` — Total PnL, Avg PnL, Trade Volume by sentiment
2. `chart2_win_rate.png` — Win rate by sentiment
3. `chart3_long_short_bias.png` — Long vs Short directional bias
4. `chart4_monthly_pnl_fg.png` — Monthly PnL vs Fear/Greed score
5. `chart5_top_coins_traders.png` — Top 10 coins and traders
6. `chart6_leverage_analysis.png` — Leverage impact on returns

## How to Run
```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook Bitcoin_Sentiment_Trading_Analysis.ipynb
```

## Tools Used
- Python, Pandas, NumPy, Matplotlib, Seaborn
- Data: Hyperliquid DEX + Alternative.me Fear & Greed Index
