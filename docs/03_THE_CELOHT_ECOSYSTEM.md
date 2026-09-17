# 03 — The CeloHT Ecosystem

## Public repositories (Celo-HaiTi organization)

The following repositories were identified as publicly visible under the
`Celo-HaiTi` GitHub organization during this rebuild. See
[architecture/REPOSITORY_MAP.md](../architecture/REPOSITORY_MAP.md) for the full table with purpose, layer,
and status. This list should be re-verified periodically, since repository
visibility and activity can change.

- `CeloHT` — flagship documentation/policy repository
- `celoht-docs` — official documentation (architecture, governance, APIs,
  education, whitepaper, roadmap, RFCs)
- `celoht-governance` — governance layer reference implementation
  (proposal lifecycle, RBAC, treasury approval with timelock, audit log)
- `celoht-smart-contracts` — Celo smart contracts (Agent Network, Service
  Payments, Education, Reforestation, Governance) — testnet
- `celoht-research` — research papers, RFCs, technical specifications
- `celoht-siteweb` — public website (celoht.com)
- `celoht-demo` — interactive investor/grant-reviewer demo (explicitly
  labeled as simulated, not connected to live blockchain activity)

Repositories referenced in prior planning material but **not independently
confirmed as publicly visible** during this rebuild (`celoht-dapp`,
`celoht-backend`, `celoht-indexer`, `celoht-supabase`, `celoht-brand`)
are marked `EXTERNAL VERIFICATION REQUIRED` in
[architecture/REPOSITORY_MAP.md](../architecture/REPOSITORY_MAP.md) rather than asserted as active.

## How the pieces relate

Documentation and governance logic live in `CeloHT`, `celoht-docs`, and
`celoht-governance`. Protocol logic lives in `celoht-smart-contracts`.
Public-facing presentation lives in `celoht-siteweb` and `celoht-demo`
(the latter explicitly a simulation, not a production surface). This book
is a new, separate repository (`celoht-investor-book`) that synthesizes
and cross-references the above rather than duplicating their content.
