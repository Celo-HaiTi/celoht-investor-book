# 24 — Risks

This is a factual, non-sensational risk list. No probability estimates are
assigned; none were independently derivable during this rebuild.

- **Blockchain infrastructure dependency** — CeloHT depends on the Celo
  network, which it does not control.
- **RPC dependency** — application functionality depends on third-party
  RPC providers.
- **Wallet dependency** — transaction signing depends on third-party
  wallet software (MiniPay, Valora, WalletConnect-compatible wallets).
- **Smart contract security** — current contracts are testnet-only and
  explicitly not independently audited; mainnet deployment without an
  audit would carry materially higher risk.
- **Regulatory / legal uncertainty** — financial-services-adjacent
  activity (agent-based cash-to-USDm conversion) may be subject to
  evolving regulation in Haiti and elsewhere; this book does not assert
  any specific compliance status.
- **Adoption risk** — the agent network and education programs require
  sustained community adoption to achieve their stated goals.
- **Operational infrastructure risk** — reliance on hosted infrastructure
  (e.g., Supabase/PostgreSQL, if in use) introduces third-party
  operational dependency.
- **Funding constraints** — as with most early-stage open-source
  initiatives, continued development depends on securing funding; no
  funding runway is asserted in this edition.
- **Data verification risk** — impact and adoption metrics (education,
  agents, reforestation) require ongoing independent verification to
  remain credible; see [docs/22_METRICS.md](./22_METRICS.md).
- **Ecosystem dependency** — changes in Celo's own roadmap, fee structure,
  or supported wallets could affect CeloHT's product.

This list is not exhaustive and should be reviewed alongside
[docs/25_DUE_DILIGENCE.md](./25_DUE_DILIGENCE.md).
