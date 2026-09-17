# Repository Map

Verified via public GitHub research (repository pages, wiki, and one
release) as part of preparing [publication/celoht-investor-book.pdf](../publication/celoht-investor-book.pdf).
Column "Status" reflects confirmation depth, not code quality. See
[publication/celoht-investor-book.pdf](../publication/celoht-investor-book.pdf), Appendix D, for full profiles.

| Repository | Purpose | Layer | Status |
|---|---|---|---|
| `CeloHT` | Flagship documentation & organizational policy (60+ root files: governance, business, treasury, security, brand, legal) + project wiki | Documentation & Policy | `VERIFIED` public |
| `celoht-docs` | Official technical & governance documentation, litepaper/whitepaper, RFCs | Documentation & Policy | `VERIFIED` public |
| `celoht-research` | Research papers, claims classification (verified/reported/planned/unverified) | Documentation & Policy | `VERIFIED` public |
| `celoht-brand` | Visual identity and brand assets (referenced from celoht-docs) | Documentation & Policy | `VERIFIED` existence (via citation); not opened page-by-page |
| `celoht-governance` | Governance reference implementation: proposal lifecycle, RBAC, treasury timelock, audit log | Governance & Protocol | `VERIFIED` public; `IMPLEMENTED` (code-level); production deployment `BLOCKED BY EXTERNAL DEPENDENCY` per source |
| `celoht-smart-contracts` | Agent Network, Service Payments, Education, Reforestation, Governance contracts | Governance & Protocol | `VERIFIED` public; `TESTNET` only (Celo Sepolia, chain ID 11142220); explicitly not audited |
| `celoht-dapp` | User-facing frontend (static, GitHub Pages-hosted); explicitly does NOT hold Solidity contracts | Application Layer | `VERIFIED` public; Celo Sepolia testnet only |
| `celoht-backend` | Wallet authentication / API boundary; tagged release v0.1.0 found | Application Layer | `VERIFIED` public; at least one tagged release |
| `celoht-admin` | Internal operations dashboard (treasury, governance, education, reforestation reporting) | Application Layer | `VERIFIED` public; explicitly fails closed without verified data providers |
| `celoht-siteweb` | Public marketing website (celoht.com), Next.js | Presentation | `VERIFIED` public and live |
| `celoht-demo` | Simulated investor/grant-reviewer demo — explicitly non-production | Presentation | `VERIFIED` public; explicitly simulated |
| `celoht-investor-book` | This repository | Documentation | New (this edition) |
| `celoht-indexer` | Referenced in `celoht-governance` as "owner of on-chain projections" | Infrastructure | `EXTERNAL VERIFICATION REQUIRED` — not independently located as a separate public repo |
| `celoht-supabase` | Referenced in `celoht-governance` as the canonical migrations process | Infrastructure / Data | `EXTERNAL VERIFICATION REQUIRED` — not independently located as a separate public repo |

## Maintenance note

This table should be re-verified whenever repositories are added, renamed,
archived, or made private, since visibility can change independently of
this document.
