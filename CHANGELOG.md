# Changelog

All notable changes to the CeloHT Investor & Open Source Project Book are documented here.

## [1.0.2] — August 2026

### Editorial pass: punctuation and prose style
- **79 em dashes found across the manuscript, all removed.** None were deleted outright: each was individually reviewed in context and rewritten using natural punctuation (commas, colons, semicolons, or parentheses) so the surrounding sentence still reads correctly
- 6 structural em dashes in Part labels ("Part I, Foundations") and 4 in figure captions converted to colons for a cleaner, more conventional look
- 1 additional em dash found only in the rendered PDF text (a unicode-escaped instance that a plain-text search had missed) and corrected in a follow-up pass, confirming the fix with a full-text extraction of all 64 pages, not just a source-code search
- Pull-quote attribution style changed from an em-dash lead-in to parenthetical, e.g. "(Johnny Dubic, Founder)"
- Scanned for common AI-cliché phrases ("rapidly evolving world," "it is important to note," "revolutionary," "cutting-edge," "game-changing," "unlocking unprecedented"): none were found in the manuscript

### Verification method
Every claimed fix was checked two ways: a source-level search across all chapter files, and a second independent search across plain text extracted from the final rendered PDF, since source-level searches can miss encoding differences that only surface at render time.

### Repetition audit
A frequency scan across the manuscript flagged "consistent with" as an overused phrase (19 occurrences in 64 pages). 9 were rewritten with natural alternatives ("in keeping with," "in line with," "following," "matching," "reflects," "appropriate to"), leaving 10 in place where the original phrasing remained the clearest choice. This was a targeted fix, not a full line-by-line rewrite of the manuscript's prose; a complete sentence-level editorial pass (varying structure and rhythm throughout all 55 chapters) remains a larger, separate undertaking if wanted.

## [1.0.1] — August 2026

### Terminology migration: cUSD → USDm
Celo's native stablecoin (formerly Celo Dollar / cUSD) was rebranded to **USDm (Mento Dollar)** by Mento Labs in December 2025 — verified independently against CoinGecko, CryptoRank, and Celo's own announcement, not merely asserted.

- **16 occurrences found**, all reviewed in context (not a blind find-and-replace)
- **11 replaced** with "USDm" where the term refers to current or forward-looking usage
- **5 preserved as intentional historical references**, each explicitly labeled (e.g. "USDm... formerly known as cUSD," "the direct successor to Celo Dollar (cUSD)"), so historical and current terminology are never ambiguous
- Glossary entry re-alphabetized: "cUSD" entry removed, "USDm" entry added in correct alphabetical position with full historical note
- Chapter 8 ("Why Celo Blockchain") expanded with one additional sentence explaining the rebrand directly, since this is the book's main technical reference point for the term

### Important caveat
At the time of this migration, CeloHT's own GitHub repositories (`celoht-smart-contracts` and others) still carried "cusd" in their topic tags and had not yet completed their own migration to USDm. This book was updated ahead of that repository-level update, on the understanding that the repositories would be updated to match. If the repositories have not yet been updated when this book is published, that inconsistency should be resolved before wide distribution.

## [1.0.0] — August 2026

### Added
- Complete 55-chapter manuscript merged into a single 63-page publication-ready document
- Automatically-verified Table of Contents with accurate page numbers
- Running header/footer with page numbers throughout
- Four original diagrams replacing all figure placeholders (see below)

### Diagrams added (replacing placeholders)
- **Figure 5.1** — Three-problem framework (language barrier, banking infrastructure, technical talent), illustrating the book's own conceptual argument
- **Figure 21.1** — CeloHT repository architecture, built directly from the verified eight-repository structure on github.com/Celo-HaiTi
- **Figure 22.1** — CeloHT dApp prototype navigation flow, explicitly labeled "PROTOTYPE — all interactions shown are simulated, not connected to mainnet" to avoid any implication of live functionality
- **Figure 52.1** — CeloHT ecosystem map connecting the three pillars, the eight-repository codebase, and the FreClean relationship, based on content already established elsewhere in the manuscript

No diagram introduces metrics, deployments, users, or integrations not already stated and verified elsewhere in the book.

### Corrected (verified against github.com/Celo-HaiTi)
- Repository count corrected from six to **eight** public repositories throughout the manuscript (Chapters 13, 14, 16, 21, 30, 38, 46, 52), with names and purposes matched to the live GitHub organization: `CeloHT`, `celoht-docs`, `celoht-research`, `celoht-siteweb`, `celoht-dapp`, `celoht-smart-contracts`, `celoht-brand`, `.github`
- Governance model corrected in Chapters 14, 15, 16, 46, and 48 to reflect the actual documented structure — a **Foundation Director**, **Maintainer Council**, and **Community Contributors** — rather than sole founder authority
- Technical Architecture table (Chapter 21) rebuilt to list the real eight repositories with accurate purposes and primary technologies

### Removed
- All 51 "Key Takeaways" summary boxes removed for uninterrupted investor readability, per direct request

### Unchanged
- Core narrative, chapter structure, title, and professional tone
- No-token / no-cryptocurrency positioning throughout
- Front matter (Foreword, Letter from the Founder, Executive Summary)

### Known open items (require human verification before final sign-off)
- Content of the 60+ individual policy files in the `CeloHT` repository (TREASURY.md, LEGAL_STATUS.md, BUSINESS.md, FINANCIAL_REPORTS.md, etc.) has not been individually cross-checked line-by-line against this book's claims
- Live/deployed status of `celoht-dapp` and `celoht-smart-contracts` on testnet or mainnet has not been independently confirmed beyond the "prototype / simulated wallet" status already stated in the book
- No metrics in this book (people trained, transactions, revenue, agents) have external audit confirmation
- **GitHub commit, push, and release have not been performed** — this repository package is prepared locally and requires the maintainer's own `git push` and GitHub Release creation
