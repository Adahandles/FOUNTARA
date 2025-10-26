# Fountara — Water Token (WTR) Governance

This repo hosts the public website and governance artifacts for **Water Token (WTR)**.

## Canonical IDs
- **Policy ID**: `7e159ba1d6ef752b5f3ba12a97f3b46a9706687b233341cc5f83d33b`
- **Subject**: `7e159ba1d6ef752b5f3ba12a97f3b46a9706687b233341cc5f83d33b575452` ("WTR")
  - *The Subject is derived by concatenating the Policy ID with the hex-encoded ASCII string for "WTR" (`575452`). This allows readers to verify the correctness of the Subject value.*

## On‑chain scripts (placeholders)
- `scripts/treasury.multisig.json` — fill `<hw*_hash>` with 5 signer payment key hashes
- `scripts/lpdesk.locked.json` — fill `<S_lock>` (absolute slot) and signer hashes
- `policy/wtr.policy.lock.json` — fill `<policy_key_hash>` and `<S_cutoff>` (absolute slot)

## Addresses (to be filled post-audit)
See `docs/addresses.md`. Replace `<TO_BE_DEPLOYED>` with real `addr1...` after multisig creation.

## Tranche configuration
`docs/tranche.WTR-T90-2025Q4.json` provides a 90‑day Liquidity Bond example with WTR APR.

---
**Security note:** do not publish private keys. Commit only verifiable addresses, key *hashes*, and script JSON.
