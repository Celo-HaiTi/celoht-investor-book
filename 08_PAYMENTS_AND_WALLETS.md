# 08 — Payments & Wallets

## Currency terminology

- **USDm** — canonical stable-value currency for payments within CeloHT
- **CELO** — used strictly for network gas, never described as a CeloHT
  asset or governance token

The term "cUSD" is not used as current CeloHT terminology in this edition.

## Wallet strategy

CeloHT's documented wallet strategy is multi-wallet, not Valora-exclusive:

- **MiniPay** — lightweight, non-custodial wallet for stablecoin payments
  (per Celo's own documentation)
- **Valora**
- **WalletConnect-compatible wallets**

CeloHT does not claim official affiliation with MiniPay, Valora,
WalletConnect, or the Celo Foundation. Where Valora or MiniPay is
recommended to users, this book states plainly that the recommendation
does not imply affiliation unless independently verified.

## Transaction flow (as designed)

1. User connects a supported wallet to the CeloHT dApp
2. The dApp detects network and wallet compatibility
3. Payments are denominated in USDm; gas is paid in CELO
4. Failed or unsupported network/wallet states are surfaced to the user
   rather than silently failing

**Status: `PROJECT-REPORTED` design; live failure-handling behavior in
production is `EXTERNAL VERIFICATION REQUIRED`.**
