# 10 — Smart Contracts

**Source repository:** `Celo-HaiTi/celoht-smart-contracts` (public)

## What is documented

- Contract modules for: Agent Network, Service Payments, Education,
  Reforestation, and Governance
- Settlement model: USDm-only, with CELO used strictly for gas
- Governance model at the contract level: one-wallet-one-vote, no token
- Deployment target: **Celo Sepolia testnet**, chain ID **`11142220`**
- License: Apache 2.0

## Explicit status, as documented by the project itself

- Described as **"testnet-ready"**, not audited, and **not mainnet-ready**
- "DEPLOYED" and "VERIFIED" (block-explorer verification) describe the
  current Celo Sepolia testnet state only — they do **not** mean audited
  or mainnet-ready

## What this book does not do

- It does not list specific contract addresses in this edition, because
  addresses were not independently re-verified against a live block
  explorer at the time of writing. Before citing a specific deployed
  address externally, verify it directly on a Celo Sepolia block explorer
  and record the verification date in `evidence/VERIFICATION_STATUS.md`.
- It does not claim an audit has occurred. No audit firm, audit date, or
  audit report is referenced, because none was identified in public
  sources during this rebuild.

## Due-diligence checklist for this section

- [ ] Confirm current deployed contract addresses on Celo Sepolia
- [ ] Confirm whether any audit has since been commissioned or completed
- [ ] Confirm whether a mainnet deployment plan exists and its timeline
- [ ] Review `npm run validate:contracts` (or equivalent) output referenced
      in `celoht-governance`, if accessible
