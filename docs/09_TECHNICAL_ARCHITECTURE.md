# 09 — Technical Architecture

See also `docs/04_PRODUCT_ARCHITECTURE.md` for the product-level view and
`architecture/REPOSITORY_MAP.md` for the repository-to-layer mapping.

## Layers

| Layer | Responsibility | Trust boundary | Status |
|---|---|---|---|
| Smart Contracts | Agent Network, Service Payments, Education, Reforestation, Governance logic | Blockchain-trusted | `TESTNET` (Celo Sepolia, chain ID `11142220`) |
| Celo network | Settlement, gas | Blockchain-trusted (external to CeloHT) | External infrastructure — CeloHT does not control it |
| Indexer | Reads on-chain events into an application-queryable form | Infrastructure-controlled | `EXTERNAL VERIFICATION REQUIRED` |
| Backend / API | Business logic, auth boundary | Application-controlled | `EXTERNAL VERIFICATION REQUIRED` |
| Supabase / PostgreSQL | Application data storage | Infrastructure-controlled (third-party hosted) | `EXTERNAL VERIFICATION REQUIRED` |
| dApp | User-facing wallet-integrated application | User-controlled (client-side) + application-controlled (served app) | `EXTERNAL VERIFICATION REQUIRED` |
| Governance layer | Proposal lifecycle, RBAC, treasury approval with timelock, audit log | Application-controlled | `IMPLEMENTED` per source; production deployment `BLOCKED BY EXTERNAL DEPENDENCY` (runtime infrastructure not yet configured, per source) |

## Failure modes and dependencies

- **RPC dependency:** dApp and indexer functionality depends on Celo RPC
  availability, which is external infrastructure not controlled by CeloHT.
- **Wallet dependency:** transaction signing depends on third-party wallet
  software (MiniPay, Valora, WalletConnect-compatible wallets).
- **Hosted data dependency:** if Supabase/PostgreSQL is used as described,
  application data availability depends on that hosted service.

## What "production-ready" means in this book

This book never asserts "100% production ready." Instead it uses a
readiness ladder, applied per component:

`DOCUMENTED → IMPLEMENTED → TESTED → INTEGRATED → EXTERNALLY VERIFIED → PRODUCTION VERIFIED`

No component in this edition is labeled `PRODUCTION VERIFIED` absent a
specific, dated, sourced confirmation.
