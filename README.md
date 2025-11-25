# raju_binance_bot
A comprehensive CLI-based trading bot for Binance USDT-M Futures with support for multiple order types, advanced strategies, and robust logging.

## 📋 Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Order Types](#order-types)
- [Advanced Strategies](#advanced-strategies)
- [Logging](#logging)
- [Safety & Best Practices](#safety--best-practices)
- [Troubleshooting](#troubleshooting)

## ✨ Features

### Core Orders (Mandatory)
- ✅ **Market Orders** - Instant execution at current market price
- ✅ **Limit Orders** - Execute at specified price or better

### Advanced Orders (Bonus)
- ✅ **Stop-Limit Orders** - Trigger limit order when stop price is hit
- ✅ **OCO Orders** - One-Cancels-the-Other (Take Profit + Stop Loss)
- ✅ **TWAP Strategy** - Time-Weighted Average Price execution
- ✅ **Grid Trading** - Automated buy-low/sell-high within price range

### Additional Features
- 🔒 Input validation for all parameters
- 📝 Structured logging with timestamps
- 🔐 Secure API key management
- 🧪 Testnet support for paper trading
- 💰 Account balance and position monitoring
- 📊 Real-time price information

## 📁 Project Structure

```
binance_chatbot.py/
├── src/
│   ├── utils/
│   │   ├── __init__.py
│   │   ├── config.py          # API configuration & client management
│   │   ├── logger.py          # Structured logging system
│   │   └── validator.py       # Input validation utilities
│   ├── advanced/
│   │   ├── __init__.py
│   │   ├── stop_limit.py      # Stop-limit order implementation
│   │   ├── oco.py             # OCO order implementation
│   │   ├── twap.py            # TWAP strategy implementation
│   │   └── grid_orders.py     # Grid trading implementation
│   ├── market_orders.py       # Market order module
│   ├── limit_orders.py        # Limit order module
│   └── main.py                # Main CLI interface
├── bot.log                    # Log file (auto-generated)
├── .env                       # Environment variables (create from .env.example)
├── .env.example               # Example environment configuration
├── requirements.txt           # Python dependencies
├── README.md                  # This file
└── report.pdf                 # Analysis and documentation
```
