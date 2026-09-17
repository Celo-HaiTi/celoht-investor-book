# 06 — Agent Network

The Agent Network is a community-rooted network of local agents intended
to provide cash-to-USDm conversion and digital payment support.
**Status: architecture `PROJECT-REPORTED`; live operational metrics
`EXTERNAL VERIFICATION REQUIRED`.**

## Described components

- Agent onboarding
- Wallet onboarding for end users
- Cash-to-USDm and USDm-to-cash conversion flows
- Agent identity and (where implemented) DID-based verification
- Transaction assistance for users new to digital wallets

## What is not claimed in this edition

- Nationwide coverage
- A specific number of active agents
- Transaction volume or agent revenue

Any of the above should only be added once sourced from a dated,
verifiable record (e.g., an on-chain data export, a signed partner report,
or a published project update), and should carry an explicit
`verified` / `reported` / `estimated` label per [docs/22_METRICS.md](./22_METRICS.md).

## Smart contract support

The `celoht-smart-contracts` repository documents an Agent Network
contract module as part of its testnet-deployed stack. This confirms the
protocol-level design exists; it does not by itself confirm live agent
operations. See [docs/10_SMART_CONTRACTS.md](./10_SMART_CONTRACTS.md).
