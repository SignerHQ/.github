<div align="center">

<br>

# Signer.io

### The world's first Isolated Wallet

**More secure than hardware wallets. No device to buy. Use any spare computer as your signer - it never touches the internet.**

<br>

[![Blockchains](https://img.shields.io/badge/Blockchains-117+-0066ff?style=for-the-badge)](#-117-blockchains)
[![Languages](https://img.shields.io/badge/Languages-42-7c3aed?style=for-the-badge)](#-42-languages)
[![Formats](https://img.shields.io/badge/Import_Formats-40+-00b4d8?style=for-the-badge)](#-40-import-formats)
[![License](https://img.shields.io/badge/License-PolyForm_Shield-e5e5e5?style=for-the-badge)](LICENSE)

<br>

*Open code. Free forever.*

<br>

[Website](https://www.signer.io) · [Source Code](https://github.com/SignerHQ/signer) · [Compiler](https://github.com/SignerHQ/signer-compiler) · [Universal Quantum Seed](https://github.com/SignerHQ/universal-quantum-seed)

<br>

</div>

---

<br>

## How It Works

Signer.io splits your wallet into four roles across separate devices - your private keys never touch the internet.

```
┌──────────────────┐    ┌──────────────────┐    ┌──────────────────┐    ┌──────────────────┐
│                  │    │                  │    │                  │    │                  │
│     SIGNER       │◄──►│     WALLET       │◄──►│   RELAY NODE     │◄──►│      NODE        │
│    (Offline)     │    │  (App/Browser)   │    │    (Online)      │    │    (Online)      │
│                  │    │                  │    │                  │    │                  │
│  Seeds & signing │    │  App or browser  │    │  Identity & IP   │    │  Blockchain      │
│  Keys never      │    │  No download     │    │  Load balancing  │    │  queries         │
│  leave this      │    │  required        │    │  Node discovery  │    │  Broadcasting    │
│  device          │    │  Broadcasts      │    │  Health checks   │    │  Balance checks  │
│                  │    │  signed tx       │    │                  │    │                  │
└──────────────────┘    └──────────────────┘    └──────────────────┘    └──────────────────┘
    🔒 Air-gapped        📱 App / browser   🛡️ Protects your identity      💻 Computer
```

No hardware wallet to buy. No manufacturer to trust. No supply chain to verify. Take any spare computer, disconnect it from the internet, and it becomes your Signer. The Wallet works as an app or in any browser - no download required, just connect to your Signer. Relay Nodes protect your identity and IP address by default and load balance across the network.

<br>

## Features

### 💎 117+ Blockchains

Bitcoin, Ethereum, Solana, Cosmos, Polkadot, XRP, Cardano, Monero, and 110+ more. All major blockchain families supported natively - no plugins, no companion apps, no limitations.

### 🔄 40+ Import Formats

BIP39, SLIP39, Aezeed, Electrum, WIF, Monero seeds, Codex32, SeedQR, SSKR, keystores, and dozens more. Migrate from any wallet seamlessly.

### 🌍 42 Languages

Full UI in 42 languages across 10 writing systems. Arabic, Chinese, Hindi, Japanese, Korean, Russian, and more. True global accessibility - not just translated menus.

### 🧬 Quantum-Ready

Post-quantum signatures with **ML-DSA-65** (FIPS 204) and **SLH-DSA** (FIPS 205). Hardened 6-layer key derivation with PBKDF2 + Argon2id. Your keys are ready for tomorrow.

### 🍯 Hidden Profiles

Unlimited independent accounts derived from a single seed. Profile passwords produce completely unrelated keys. No mathematical way to detect hidden profiles exist - plausible deniability by design.

<br>

## Universal Quantum Seed

**One seed. Any language. Any format.**

256 universal icons mapped to 42 languages. Write your backup in English, recover it in Japanese. Or skip words entirely - just pick the icons.

| | | | | | | | | |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 🇬🇧 `dog` | 🇪🇸 `perro` | 🇫🇷 `chien` | 🇩🇪 `Hund` | 🇯🇵 `犬` | 🇰🇷 `개` | 🇷🇺 `собака` | 🇸🇦 `كلب` | 🐕 |

- **272-bit entropy** with 16-bit checksum - survives Grover's algorithm with 136-bit post-quantum security margin
- **Cross-language recovery** - write in Spanish, recover in Arabic, mix languages freely
- **Accent-insensitive** - `corazón` = `corazon`, emoji input supported
- **Plausible deniability** - your backup looks like random notes, not a crypto wallet

→ [Full documentation](https://github.com/SignerHQ/universal-quantum-seed)

<br>

## Node Network

Decentralized infrastructure for blockchain queries, broadcasting, and balance checks. Your keys stay on the Signer - the Node handles everything else.

```
  SIGNER (offline)
     │ BT / USB / WiFi
  WALLET APP
     │ HTTPS
  RELAY NODE ─── Identity & IP protected by default, load balanced, health-checked
     │
  NODE ─── 117+ blockchains, real-time data
```

**Relay Node** - sits between users and the blockchain nodes, protecting IP addresses by default:

| Feature | Description |
|:---|:---|
| **Identity & IP Protection** | Your identity and real IP are never exposed to blockchain nodes - Relay handles all outbound requests |
| **Load Balancing** | Weighted distribution across available nodes with automatic failover |
| **Circuit Breaker** | Exponential backoff isolates unhealthy nodes. Healthy nodes absorb load. Zero downtime |
| **Connection Pooling** | Persistent HTTP keep-alive pools with token bucket rate limiting |
| **Open Discovery** | Relays accept new nodes via verified discovery - health-checked and ban-capable |
| **WebSocket Streaming** | Real-time push updates for watched addresses without polling |
| **API Key Management** | Per-profile keys with per-coin access control, firewall rules, and request logging |

<br>

## Signer.io vs. Hardware Wallets

| | Signer.io | Hardware Wallets |
|:---|:---:|:---:|
| Keys isolated from internet | ✅ | ✅ |
| Dedicated signing device | ✅ | ✅ |
| No device purchase required | ✅ | ❌ |
| No supply chain trust required | ✅ | ❌ |
| Fully open code - no hidden firmware | ✅ | ⚠️ |
| 117+ blockchains natively | ✅ | ⚠️ |
| 40+ seed/key import formats | ✅ | ❌ |
| Post-quantum cryptography | ✅ | ⚠️ |
| Hidden profiles / plausible deniability | ✅ | ❌ |
| 42 languages / 10 writing systems | ✅ | ❌ |
| Built-in Tor hidden services | ✅ | ⚠️ |
| Wallet works as app or browser - no download | ✅ | ❌ |
| Free forever | ✅ | ❌ |

<br>

## Platforms

| | Signer (Offline) | Wallet App | Node |
|:---|:---:|:---:|:---:|
| **Windows** | ✅ | ✅ | ✅ |
| **macOS** | ✅ | ✅ | ✅ |
| **Linux** | ✅ | ✅ | ✅ |
| **Any device (app or browser)** | - | ✅ | - |

<br>

## Repositories

| Repository | Description |
|:---|:---|
| [**Signer**](https://github.com/SignerHQ/signer) | The main wallet - offline signing, 117+ blockchains, PySide6 GUI |
| [**Universal Quantum Seed**](https://github.com/SignerHQ/universal-quantum-seed) | 256-icon, 42-language, quantum-safe seed phrase system |
| [**Signer Compiler**](https://github.com/SignerHQ/signer-compiler) | One-command build tool for Windows, macOS, and Linux |

<br>

## License

[PolyForm Shield 1.0.0](https://polyformproject.org/licenses/shield/1.0.0) - Copyright © 2026 Signer.io

<br>

---

<div align="center">

**Your keys. Your rules.**

Signer.io is free, open code, and built for everyone.<br>No company controls your wallet. No device required. No compromises.

<br>

⭐ Star our repos if you believe in open, secure, and accessible crypto.

</div>
