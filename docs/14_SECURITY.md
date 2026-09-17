# 14 — Security

## Smart contract security

- Deployed to **Celo Sepolia testnet only**
- Explicitly described by the project as **not independently audited**
- **Mainnet deployment requires an independent security audit and
  operational approval**, per the project's own documentation — this book
  treats mainnet readiness as unmet until that audit is documented

## Distinctions this book enforces

| Term | Meaning used in this book |
|---|---|
| Audited | An independent, named audit firm has reviewed the code and a report exists |
| Internally reviewed | Project contributors have reviewed the code; no independent audit |
| Not independently audited | No audit, internal or external, is claimed |

No component in this edition is labeled "Audited" without a named auditor
and report reference.

## Application-layer security (status: EXTERNAL VERIFICATION REQUIRED)

The following areas are relevant to a full security review but were not
independently verified during this rebuild:

- Authentication / authorization boundary (backend/API)
- Secret handling and credential storage
- Database access controls (Supabase/PostgreSQL, if in use)
- RPC security and rate limiting
- Dependency vulnerability scanning
- Incident response process

## Vulnerability disclosure

If a documented security disclosure process exists in a Celo-HaiTi
repository (e.g., a `SECURITY.md`), it should be linked from here once
confirmed. This edition does not invent a disclosure process or contact
channel that was not independently verified.
