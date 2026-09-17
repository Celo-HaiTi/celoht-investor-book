# CeloHT — Ecosystem & Investor Book

**Status:** v1.0.0 — First canonical edition (zero-based build)
**Canonical organization:** [Celo-HaiTi](https://github.com/Celo-HaiTi)
**Canonical project name:** CeloHT
**Currency terminology:** USDm (payments) · CELO (gas)
**Founder:** Johnny Dubic

This repository is the authoritative, investor- and public-facing explanation of
CeloHT: what it is, what has been built, what remains unfinished, and how an
external reviewer can independently verify every claim made here.

CeloHT is an open-source Haitian Web3 initiative focused on financial
inclusion, blockchain education, digital payments, and entrepreneurship
within the Celo ecosystem. It is organized around three public pillars:

- **Education** — Web3, financial literacy, and digital security education
- **Agents** — a community-rooted agent network for cash-to-USDm conversion
  and digital payment support
- **Reforestation** — measurable, transparently reported environmental
  restoration linked to community development

CeloHT is **not** a blockchain, **not** a cryptocurrency, and **not** an
investment product. There is no native CeloHT token. See
[`NO_TOKEN_POLICY.md`](./NO_TOKEN_POLICY.md).

## How to read this repository

| If you are a... | Start here |
|---|---|
| Investor / grant reviewer | [`BOOK.md`](./BOOK.md), then [`docs/25_DUE_DILIGENCE.md`](./docs/25_DUE_DILIGENCE.md) |
| Technical reviewer / engineer | [`docs/09_TECHNICAL_ARCHITECTURE.md`](./docs/09_TECHNICAL_ARCHITECTURE.md), [`architecture/REPOSITORY_MAP.md`](./architecture/REPOSITORY_MAP.md) |
| Journalist / researcher | [`docs/01_IDENTITY_AND_MISSION.md`](./docs/01_IDENTITY_AND_MISSION.md), [`docs/28_SOURCES.md`](./docs/28_SOURCES.md) |
| Prospective contributor | [`community/CONTRIBUTING.md`](./community/CONTRIBUTING.md) |

## What this repository is not

- It is not the source of truth for application code (see `celoht-dapp`,
  `celoht-smart-contracts`, `celoht-backend`, `celoht-indexer` in the
  Celo-HaiTi organization).
- It is not a token sale document. CeloHT has no token, no ICO, no presale.
- It is not a marketing brochure. Every substantive claim carries a
  verification status (see [`evidence/VERIFICATION_STATUS.md`](./evidence/VERIFICATION_STATUS.md)).

## Verification model

Every claim in this book is labeled with one of the following statuses:

`VERIFIED` · `PROJECT-REPORTED` · `IMPLEMENTED` · `TESTNET` ·
`IN DEVELOPMENT` · `PLANNED` · `EXTERNAL VERIFICATION REQUIRED` · `UNKNOWN`

A status of `PLANNED` never becomes `LIVE` without evidence. A status of
`TESTNET` never becomes `MAINNET` without an independent audit and
documented mainnet deployment. See [`docs/28_SOURCES.md`](./docs/28_SOURCES.md)
for the full source list this edition was built from.

## License

Apache License 2.0 (consistent with other Celo-HaiTi repositories such as
`celoht-smart-contracts` and `celoht-research`). See [`LICENSE`](./LICENSE).

## Publication

A full narrative edition of this book — with diagrams, a table of contents,
and page numbers — is available in [`publication/`](./publication/) as
both a Word document (`celoht-investor-book.docx`) and a PDF
(`celoht-investor-book.pdf`). The Markdown files in this repository remain
the canonical, most granular source; the publication is generated from the
same research and is meant for sharing with investors and institutions who
prefer a single formatted document.

## Rebuild notes

This edition was built from zero, directly researched across the public
Celo-HaiTi organization. See [`REBUILD_AUDIT.md`](./REBUILD_AUDIT.md) for
what was verified, what remains unverified, and what a reviewer with
direct repository access should confirm next.
