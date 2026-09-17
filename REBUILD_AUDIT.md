# REBUILD_AUDIT.md

## Rebuild status

`celoht-investor-book` did not exist as a public repository prior to this
work. This is a **first canonical build**, produced from zero and
cross-referenced against the public Celo-HaiTi organization rather than
edited from any prior corpus.

## Research scope

Twelve public repositories were directly reviewed: `CeloHT` (flagship,
including its wiki), `celoht-docs`, `celoht-governance`,
`celoht-smart-contracts`, `celoht-research`, `celoht-siteweb`,
`celoht-dapp`, `celoht-backend`, `celoht-admin`, `celoht-brand`, and
`celoht-demo`, plus one tagged release (`celoht-backend v0.1.0`).
`celoht-indexer` and `celoht-supabase` are referenced inside
`celoht-governance` but were not independently located as separate public
repositories; they are marked `EXTERNAL VERIFICATION REQUIRED` throughout.

## Rebuilt (canonical documents)

- [README.md](./README.md), [BOOK.md](./BOOK.md), [NO_TOKEN_POLICY.md](./NO_TOKEN_POLICY.md), [LICENSE](./LICENSE)
- `docs/00` through `docs/28` (see the published book's table of contents
  for the final chapter list and numbering)
- [architecture/REPOSITORY_MAP.md](./architecture/REPOSITORY_MAP.md)
- [evidence/VERIFICATION_STATUS.md](./evidence/VERIFICATION_STATUS.md)
- [community/CONTRIBUTING.md](./community/CONTRIBUTING.md)
- [publication/celoht-investor-book.docx](./publication/celoht-investor-book.docx) and `.pdf` — a full narrative
  edition with diagrams, a page-numbered table of contents, and a
  structured due-diligence checklist

## Identity verification

- "CeloHT" — `VERIFIED`
- "Celo-HaiTi" — `VERIFIED`
- "USDm" — `VERIFIED` as current terminology (not independently verified
  as a specific on-chain token contract)
- "CELO" — `VERIFIED` (Celo's native gas asset; CeloHT does not issue or
  control it)
- Founder: Johnny Dubic — `VERIFIED`, with explicit, repeated
  authority-limitation language confirmed across four independent sources

## Governance verification

Canonical source: `celoht-governance` (public repository). Founder role
and its limitations were cross-confirmed against `CeloHT/FOUNDER.md` and
`celoht-siteweb`. Quorum, approval thresholds, and production deployment
timeline were **not** independently confirmed and are marked `PENDING
CANONICAL VERIFICATION` in the governance chapter.

## Architecture verification

See [architecture/REPOSITORY_MAP.md](./architecture/REPOSITORY_MAP.md) for the full, current repository
table. `celoht-dapp`, `celoht-backend`, and `celoht-admin` were each
independently opened and reviewed rather than assumed from a secondary
description.

## Metrics verification

No education, agent-network, or reforestation metric was found with a
traceable, dated source. The metrics chapter is populated with the
reporting framework only, not with figures. This is a deliberate choice
to avoid presenting an unsourced number as fact.

## Security

- Confirmed (project-stated): smart contracts on Celo Sepolia testnet are
  not independently audited; mainnet requires an audit per the project's
  own documentation.
- Not confirmed: full application-layer security posture (auth, secrets,
  database access, RPC rate limiting, incident response) beyond what each
  repository documents about itself.

## Tests

No test, lint, build, or audit command was executed against any
Celo-HaiTi repository as part of this work, because it was performed via
public web research rather than an authenticated local clone with
execution access. This remains explicitly outstanding work for a
reviewer with direct repository access.

## External dependencies for a full verification

- Direct, authenticated repository access (for CI logs, commit history,
  and code execution)
- Confirmation of `celoht-indexer` and `celoht-supabase` as public or
  accessible-on-request repositories
- Current, dated metrics for education, agent network, and reforestation
- Current funding target / amount raised, if any
- Confirmation of deployed smart contract addresses directly against a
  live Celo Sepolia block explorer

## Known limitations of this edition

1. Built from public web access only — no local clone, so no commit
   history, CI status, or test execution was reviewed.
2. Several sub-documents from the original planning scope (`governance/`
   and `security/` subfolders, `CODE_OF_CONDUCT.md`,
   `AI_CONTRIBUTION_POLICY.md`, `MAINTAINERS.md`, `TRUST_BOUNDARIES.md`,
   `DATA_FLOW.md`) were not drafted in this pass, to avoid filling them
   with unverified content.
3. No specific metric, funding figure, or contract address is asserted,
   by design — this trades completeness for accuracy.

## Remaining work

- [ ] Obtain direct repository access to run `git status`, `npm install`,
      `npm run lint`, `npm test`, `npm run build`, `npm audit` as
      originally specified
- [ ] Confirm `celoht-indexer` and `celoht-supabase` status directly with
      maintainers
- [ ] Populate the metrics chapter with sourced figures, if/when available
- [ ] Draft remaining sub-documents listed under "Known limitations" above
- [ ] Re-verify this document and [architecture/REPOSITORY_MAP.md](./architecture/REPOSITORY_MAP.md)
      whenever repositories are added, renamed, archived, or made private
