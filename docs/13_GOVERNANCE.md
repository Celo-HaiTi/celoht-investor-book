# 13 — Governance

This section is a rewrite based on the current canonical governance source
(`Celo-HaiTi/celoht-governance`), not on any prior investor-book chapter
structure. Older governance language such as "Foundation Director →
Maintainer Council → Community Contributors" is **not** reproduced here
and should be treated as non-canonical unless independently re-confirmed.

## Founder

- **Name:** Johnny Dubic
- **Role:** Founder — recorded as permanently recognized founder in the
  project's historical and institutional record.
- **What this role is not:** CEO, Executive Director, Managing Director,
  or a role carrying unilateral executive authority.
- **Explicit limitation, as documented by the project itself:** "Permanent
  founder recognition is historical and institutional; it does not confer
  perpetual governance authority, ownership rights, veto power, or
  unilateral control."

## Voting model

- One-member-one-vote (community-governed)
- No governance token — USDm and CELO are referenced only as a
  stablecoin/gas asset, never as governance tokens ([NO_TOKEN_POLICY.md](../NO_TOKEN_POLICY.md))

## Decision process (as documented)

- Any individual may submit a proposal
- A proposal becomes an official CeloHT decision only through the
  documented collective governance process (see `celoht-governance` for
  the reference implementation: proposal lifecycle, RBAC, treasury
  approval flow with timelock, append-only audit logging)

## What remains PENDING CANONICAL VERIFICATION

The following governance details were not independently confirmed with
sufficient specificity during this rebuild and should be verified against
`celoht-governance` directly before being cited externally:

- Exact quorum and approval thresholds for proposals
- Composition and selection process for any review/approval roles
- Current deployment status of the governance system in production
  (the source repository itself states deployment is "blocked until
  runtime infrastructure is configured")
- Conflict-of-interest handling procedures

## Deployment status

`celoht-governance` describes its implementation as synchronized with the
public CeloHT architecture, with deployment blocked pending runtime
infrastructure configuration. **Status: `IMPLEMENTED` (code-level, per
source); `BLOCKED BY EXTERNAL DEPENDENCY` (production deployment).**
