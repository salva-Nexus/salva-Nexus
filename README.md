# 🛡️ SALVA Nexus

### Permissionless Payments & Identity Infrastructure

Salva is a decentralized payments and identity infrastructure designed to make blockchain applications easier to use while remaining open for anyone to build on.

The ecosystem combines **Naming, a collateral-backed on-chain Naira, and permissionless p2p liquidity** into interoperable protocol layers — abstracting much of the underlying blockchain complexity from users and applications.

---

## 💎 The Salva Ecosystem

Salva is built around three core protocol layers:

### 1. 🏷️ SNS — Salva Naming Service

A decentralized identity and naming layer for human-readable on-chain identities.

- **Human-readable:** `pay.ngns.base@cbechange`
- **Independent namespaces:** Each namespace has its own registry, owners, and records.
- **Permissionless:** Namespaces can be configured for open or owner-controlled participation.
- **Extensible:** Records can resolve to wallet addresses or other application-specific data.

---

### 2. 🪙 NGNs — Nigerian Naira Protocol

NGNs is Salva's Naira-denominated stablecoin protocol. Minted as collateralized debt — users lock up crypto assets as collateral and mint NGNS against them.

- **Collateral-backed:** Every NGNS in circulation is backed by crypto collateral locked in the protocol.
- **User-owned positions:** Anyone can deposit approved collateral and mint NGNS against it, and repay/withdraw on their own terms.
- **Price-aware:** Collateral and debt values are continuously checked against live market prices to keep the system solvent.
- **Self-correcting:** Positions that fall below a safe collateralization level can be liquidated by anyone, keeping the system fully backed.
- **Naira-native, EVM-native:** Designed around the Nigerian Naira, and usable directly by any EVM smart contract or application.

---

### 3. ⇄ Salva PEX — Salva's Permissionless P2P Exchange

A peer-to-peer liquidity protocol for exchanging crypto assets.

- **Permissionless liquidity:** Anyone can deploy their own pool.
- **Provider-defined pricing:** Liquidity providers set their own price floor and spread.
- **Floor-protected:** Pools follow live market prices but won't sell below a provider's chosen floor unless the provider explicitly allows it — protecting liquidity from bad or stale price data.
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
           SNS              NGNs           Salva PEX
        Identity        Naira Protocol      Liquidity
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
```
