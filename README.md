# 🛡️ SALVA Nexus

### Permissionless Payments & Identity Infrastructure

Salva is a decentralized payments and identity infrastructure designed to make blockchain applications easier to use while remaining open for anyone to build on.

The ecosystem combines **Naming, on-chain Naira, and decentralized p2p** into interoperable protocol layers — abstracting much of the underlying blockchain complexity from users and applications.

---

## 💎 The Salva Ecosystem

Salva is built around three core protocol layers:

### 1. 🏷️ SNS — Salva Naming Service

A decentralized identity and naming layer for human-readable on-chain identities.

SNS uses a **Factory + EIP-1167 registry architecture**, allowing namespaces to maintain independent ownership, permissions, and records while remaining interoperable through a shared routing layer.

- **Human-readable:** `charles@salva`
- **Independent namespaces:** Each namespace has its own registry and state.
- **Permissionless:** Namespaces can be configured for open or owner-controlled participation.
- **Extensible:** Records can resolve to wallet addresses or other application-specific data.

---

### 2. 🪙 NGNs — Nigerian Naira Settlement Layer

NGNs is Salva's Naira-denominated settlement infrastructure for on-chain applications.

It provides a native unit of account for Naira-based payments and financial applications across supported EVM networks.

- **Naira-native:** Designed around the Nigerian Naira.
- **EVM-native:** Integrates directly with decentralized applications and smart contracts.

---

### 3. ⇄ Salva PEX — Salva’s Permissionless p2p Exchange

A peer-to-peer liquidity protocol for exchanging Crypto Assets.

Liquidity providers can deploy their own pools, define their parameters, and provide liquidity without relying on a centralized exchange operator.

- **Permissionless liquidity:** Anyone can deploy a pool.
- **Provider-defined pricing:** Liquidity providers determine their own exchange rates.
- **Peer-to-peer:** No centralized order book or OTC desk.
- **Transparent:** Pool parameters and transactions are enforced on-chain.

---

## 🏗️ Architecture

```text
                         SALVA NEXUS
                              │
             ┌────────────────┼────────────────┐
             │                │                │
             ▼                ▼                ▼
           SNS              NGNs           Naira DEX
        Identity          Settlement        Liquidity
             │                │                │
             └────────────────┼────────────────┘
                              │
                              ▼
                    Salva Applications
                              │
             ┌────────────────┼────────────────┐
             ▼                ▼                ▼
          Wallets          Payments        Financial
                                           Applications
