# 04 — Product Architecture

CeloHT's product surface is organized around a dApp that connects a user's
wallet to three functional areas — Education, Agent Network, and
Reforestation — backed by an API/backend layer, a Supabase/PostgreSQL data
layer, an indexer that reads on-chain state, and smart contracts on Celo.

```
User
 │
 ▼
CeloHT dApp
 ├── Wallet integration (MiniPay, Valora, WalletConnect-compatible)
 ├── Education module
 ├── Agent Network module
 └── Reforestation module
 │
 ▼
Backend / API
 │
 ▼
Supabase / PostgreSQL
 │
 ▲
Indexer  (reads on-chain events/state)
 │
 ▼
Celo network
 │
 ▼
Smart Contracts (Celo Sepolia testnet)
```

**Status:** This diagram reflects the architecture as publicly described
across `celoht-governance` and `celoht-smart-contracts`. **Status label per
component:**

| Component | Status |
|---|---|
| Smart contracts | `TESTNET` (Celo Sepolia, chain ID 11142220) |
| Governance layer | `IMPLEMENTED` (per source), deployment `BLOCKED BY EXTERNAL DEPENDENCY` (runtime infrastructure not yet configured, per source) |
| dApp / Backend / Indexer / Supabase | `EXTERNAL VERIFICATION REQUIRED` — referenced in planning material; not independently confirmed as public, deployed repositories during this rebuild |

Do not treat any component above as production-verified unless a dated,
sourced confirmation is added to `evidence/VERIFICATION_STATUS.md`.
