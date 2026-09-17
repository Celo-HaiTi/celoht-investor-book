# CeloHT — Ecosystem Book

*Canonical edition v1.0.0 — built from zero, sourced from public Celo-HaiTi
repositories. See [`docs/28_SOURCES.md`](./docs/28_SOURCES.md) for the
complete source list and [`evidence/VERIFICATION_STATUS.md`](./evidence/VERIFICATION_STATUS.md)
for the verification key used throughout.*

## Executive Summary

CeloHT is an open-source, community-driven initiative building financial
inclusion, blockchain education, and reforestation programs for Haiti on
the Celo ecosystem. It is not a blockchain, not a cryptocurrency, and not
an investment product — it is an application and community layer built on
top of Celo, using USDm for payments and CELO for network gas.

The project is organized around three public pillars — **Education**,
**Agent Network**, and **Reforestation** — supported by a technical stack
that includes a dApp, smart contracts (currently deployed to the Celo
Sepolia testnet), a backend/API layer, an indexer, and a Supabase/PostgreSQL
data layer. **Status: `IMPLEMENTED`/`TESTNET`** components exist; **no
component in this book is described as mainnet-production-verified unless
explicitly labeled `PRODUCTION VERIFIED`.**

Founder **Johnny Dubic** is permanently recognized as CeloHT's founder.
Founder recognition is historical/institutional and does not confer
unilateral governance authority — see [`docs/13_GOVERNANCE.md`](./docs/13_GOVERNANCE.md).

## 1. What is CeloHT?

CeloHT is an open-source Haitian Web3 initiative focused on financial
inclusion, blockchain education, digital payments, and entrepreneurship
within the Celo ecosystem. **Status: `PROJECT-REPORTED`, consistent across
all inspected Celo-HaiTi repositories.**

## 2. Why CeloHT Exists

Haiti faces well-documented structural barriers to formal financial
services: limited banking infrastructure, high remittance costs, and
uneven access to digital financial literacy. CeloHT's stated thesis is
that a mobile-first, stablecoin-settled payment rail — paired with local
agents who bridge cash and digital value — can lower the cost of financial
participation, while an education layer builds the literacy required to
use it safely. **Status: project thesis, `PROJECT-REPORTED`; independent
macro-level impact studies are `EXTERNAL VERIFICATION REQUIRED`.**

## 3. The CeloHT Ecosystem

```
CeloHT
│
├── Education          — Web3, financial literacy, digital security
├── Agent Network       — cash-to-USDm conversion, payment support
├── Reforestation       — financed/planted/verified environmental restoration
├── Technology          — dApp, smart contracts, backend, indexer, data layer
├── Governance          — one-member-one-vote, no governance token
└── Open Source Community — public repositories under Celo-HaiTi
```

Do not read CeloHT as a generic "Web3 startup." Its scope is intentionally
narrow: three pillars, no token, no proprietary blockchain claim.

## 4. Product Pillars

### 4.1 Education
Web3, financial literacy, and digital security education, delivered
primarily in Haitian Creole. **Status: `PROJECT-REPORTED` for curriculum
existing; specific course completion numbers are `EXTERNAL VERIFICATION
REQUIRED` unless sourced — see `docs/22_METRICS.md`.**

### 4.2 Agent Network
A community-rooted network of local agents intended to provide
cash-to-USDm conversion and digital payment support. **Status: architecture
`PROJECT-REPORTED`; live agent count, geographic coverage, and transaction
volume are `EXTERNAL VERIFICATION REQUIRED` — do not assume nationwide
coverage or active agent volume without a current, sourced figure.**

### 4.3 Reforestation
Environmental restoration linked to community development, with a stated
intent toward transparent reporting. **Status: mechanism `PROJECT-REPORTED`;
trees financed vs. planted vs. independently verified must be reported
separately — see `docs/07_REFORESTATION.md`. No impact dashboard numbers
are asserted in this edition absent a sourced figure.**

## 5. Technology

CeloHT's stack, as organized across the public Celo-HaiTi organization,
separates the application layer from Celo network infrastructure:

```
User
 │
 ▼
CeloHT dApp  (wallet integration: MiniPay, Valora, WalletConnect-compatible)
 │
 ▼
Backend / API
 │
 ▼
Supabase / PostgreSQL
 │
 ▲
Indexer
 │
 ▼
Celo network
 │
 ▼
Smart Contracts (Celo Sepolia testnet — chain ID 11142220)
```

**Status: architecture as `PROJECT-REPORTED`/`IMPLEMENTED` per public repo
descriptions (`celoht-governance`, `celoht-smart-contracts`); production
(mainnet) deployment status is `EXTERNAL VERIFICATION REQUIRED`.** Smart
contracts are described publicly as testnet-ready and explicitly **not**
audited or mainnet-ready; see `docs/10_SMART_CONTRACTS.md`.

## 6. Governance

CeloHT uses a one-member-one-vote governance model with no governance
token. Johnny Dubic holds permanent founder recognition, which is
explicitly documented (in the project's own governance repository) as
historical/institutional and **not** conferring perpetual governance
authority, ownership rights, veto power, or unilateral control. See
`docs/13_GOVERNANCE.md` for the full breakdown and what remains pending
canonical verification.

## 7. Security

Smart contracts deployed to Celo Sepolia testnet are explicitly documented
by the project as **not independently audited** and **not mainnet-ready**.
This book does not claim an audit that has not occurred. See
`docs/14_SECURITY.md`.

## 8. Business Model & Funding

CeloHT does not currently report independently verified revenue. Funding
is described in terms of organizational/project financing rather than
investment or token sale. See `docs/19_BUSINESS_MODEL.md` and
`docs/20_FUNDING.md`. Any specific funding target must be confirmed against
a current, dated source before being cited externally.

## 9. Risks

See `docs/24_RISKS.md` for a non-exhaustive list including blockchain
infrastructure dependency, wallet/RPC dependency, regulatory uncertainty,
adoption risk, smart contract security (unaudited testnet status),
funding constraints, and data verification limitations.

## 10. Roadmap

See `docs/23_ROADMAP.md`, which separates completed, in-progress, planned,
and externally-dependent work. No planned item is represented as completed.

## 11. Due Diligence

See `docs/25_DUE_DILIGENCE.md` for a structured checklist an external
reviewer can use to independently verify every claim in this book.

## 12. How to Contribute

See `community/CONTRIBUTING.md`.

## 13. Sources

See `docs/28_SOURCES.md` for the complete list of public repositories and
pages this edition was built from, with fetch dates.
