# 08 Governance Boundary

**STATUS:** `READY_NOT_PUBLISHED` · `DEPLOYED_PENDING_CUTOVER` · **`TT_PRODUCTION_GO`:** NO_GO

**Language:** English (this page) | [ZH](../zh-CN/08-governance-boundary.md)

---

## TTG is

- Governance + budget program asset (25T genesis, NO-MINT)
- Not travel order settlement (USDC default)

## Country Pool / FeeRouter

- Platform fee 5% (500 bps) — governance only to change
- Active steward: 45% of platform fee to steward wallet; 55% to NEW ProjectPool
- No steward: 100% to NEW ProjectPool
- Public sale USDC → NEW ProjectPool (never Legacy P4Cap)

## Governance

- Official PM/Vault delay: **12h** NEW SoloTimelock. PATH_A set PM.timelock and Vault.admin to NEW 12h.
- Phase1 OLD 48h SoloTimelock: **LEGACY** (still 48h on-chain; not living Official delay)

## Not claimed

- RegionVault snapshot/claim end-state (83 target — not Official LIVE)
- Production GO
- Exchange listings

SSOT: docs/github-official/en/CountryFeeRouter.md · spec 83 country-fee allocation whitepaper (ZH filename in repo)
