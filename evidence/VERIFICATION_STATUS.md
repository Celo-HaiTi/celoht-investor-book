# Verification Status Registry

## Status key

- `VERIFIED` — independently confirmed against a primary, current source
- `PROJECT-REPORTED` — stated by the project consistently across sources,
  not independently re-derived
- `IMPLEMENTED` — code/design exists per source, not necessarily deployed
- `TESTNET` — deployed to a test network only
- `IN DEVELOPMENT` — actively being built, not yet complete
- `PLANNED` — intended, not yet started or not yet complete
- `EXTERNAL VERIFICATION REQUIRED` — cannot be confirmed from sources
  consulted in this edition
- `UNKNOWN` — no claim made in either direction

## Registry

| Claim | Status | Evidence | Date |
|---|---|---|---|
| Project name "CeloHT" | `VERIFIED` | Consistent across all inspected repositories | This rebuild |
| Org "Celo-HaiTi" | `VERIFIED` | GitHub organization confirmed | This rebuild |
| Three pillars: Education, Agents, Reforestation | `VERIFIED` | Consistent across all inspected repositories | This rebuild |
| No native CeloHT token | `VERIFIED` | [NO_TOKEN_POLICY.md](../NO_TOKEN_POLICY.md) referenced across repos | This rebuild |
| Founder: Johnny Dubic | `VERIFIED` | `CeloHT/FOUNDER.md`, `celoht-governance`, `celoht-siteweb` | This rebuild |
| Founder role limits (no unilateral authority) | `VERIFIED` | Explicitly stated in `celoht-governance`, `celoht-siteweb` | This rebuild |
| One-member-one-vote governance | `PROJECT-REPORTED` | `celoht-governance` README | This rebuild |
| Governance production deployment | `BLOCKED BY EXTERNAL DEPENDENCY` | Stated directly by `celoht-governance` | This rebuild |
| Smart contracts on Celo Sepolia (chain ID 11142220) | `TESTNET` | `celoht-smart-contracts` README | This rebuild |
| Smart contracts audited | `NOT AUDITED` (explicit) | `celoht-smart-contracts` README states mainnet requires independent audit | This rebuild |
| Wallet strategy: MiniPay, Valora, WalletConnect-compatible | `PROJECT-REPORTED` | Multiple repos | This rebuild |
| USDm as payment currency, CELO as gas | `PROJECT-REPORTED` | Multiple repos | This rebuild |
| Education/Agent/Reforestation live metrics | `UNAVAILABLE` | No sourced figure identified | This rebuild |
| Funding target/amount raised | `EXTERNAL VERIFICATION REQUIRED` | Not identified in sources consulted | This rebuild |
| `celoht-dapp`, `celoht-backend`, `celoht-indexer`, `celoht-supabase` as active public repos | `EXTERNAL VERIFICATION REQUIRED` | Referenced in architecture descriptions, not independently confirmed public | This rebuild |
| "USDm" as current payment terminology | `PROJECT-REPORTED` | Consistent across root-level documentation | This rebuild |

Add a new row for every material claim before it is published anywhere
under the CeloHT name.
