# vwap-trading-bot
# VWAP Trading Bot

A lightweight algorithmic trading bot that implements a VWAP (Volume Weighted Average Price) **mean reversion** strategy using a $1,000 account.

## 📈 Strategy Overview

This bot monitors selected low-priced, high-volume stocks and executes trades when the price deviates significantly from VWAP, aiming for mean reversion.

- **Buy signal**: Price drops >2% below VWAP and shows reversal signs
- **Sell signal**: Price returns to VWAP or hits target
- **Capital**: $1,000 simulated or live trading
- **Instruments**: U.S. equities under $20 with high liquidity

## 🧱 Project Structure


vwap-trading-bot/
├── main.py # Entry point
├── strategies/
│ └── vwap_mean_reversion.py
├── data/
│ └── historical/
├── backtest/
│ └── backtester.py
├── utils/
│ └── indicators.py
├── requirements.txt
├── README.md
└── .gitignore


## ✅ Features (Planned)

- [x] VWAP-based trade signals
- [ ] Paper/live trading integration (e.g. Alpaca API)
- [ ] Simple backtesting engine
- [ ] Logging & risk management

## 🚀 Quickstart

```bash
# Clone the repo
git clone https://github.com/hpatel-07/vwap-trading-bot.git
cd vwap-trading-bot

# Set up virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
