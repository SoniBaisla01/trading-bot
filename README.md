# Binance Futures Trading Bot

A simple Python trading bot for Binance Futures Testnet.

## Features

- Place MARKET orders
- Place LIMIT orders
- BUY and SELL support
- CLI input using argparse
- Logging support
- Error handling

## Project Structure

trading_bot/
│
├── bot/
│   ├── client.py
│   ├── orders.py
│   ├── validators.py
│   └── logging_config.py
│
├── logs/
├── cli.py
├── requirements.txt
├── README.md
├── .env
└── .env.example

## Installation

1. Clone repository

2. Create virtual environment

```bash
python -m venv venv
```

3. Activate virtual environment

### Windows

```bash
venv\Scripts\activate
```

4. Install dependencies

```bash
pip install -r requirements.txt
```

## Environment Variables

Create a `.env` file and add:

```env
API_KEY=your_api_key
API_SECRET=your_secret_key
```

## Run MARKET Order

```bash
python cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.001
```

## Run LIMIT Order

```bash
python cli.py --symbol BTCUSDT --side SELL --type LIMIT --quantity 0.001 --price 150000
```

## Logging

Logs are stored in:

```text
logs/trading.log
```