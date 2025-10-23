# Binance Futures Order Bot

## Overview
CLI-based trading bot for Binance USDT-M Futures supporting market, limit, and advanced orders (OCO, TWAP).

## Setup
```bash
pip install python-binance
```

## Usage
```bash
python src/market_orders.py BTCUSDT BUY 0.01
python src/limit_orders.py BTCUSDT SELL 0.01 68000
python src/advanced/oco.py BTCUSDT SELL 0.01 70000 65000
python src/advanced/twap.py BTCUSDT BUY 0.05 5 2
```

## Logging
Logs all actions in `bot.log` with timestamps and error handling.

## Structure
- src/
  - market_orders.py
  - limit_orders.py
  - advanced/
    - oco.py
    - twap.py
- bot.log
- report.pdf
- README.md
