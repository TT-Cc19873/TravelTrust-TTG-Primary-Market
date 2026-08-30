# Governance vs country pool

**STATUS:** `READY_NOT_PUBLISHED` · `DEPLOYED_PENDING_CUTOVER` · **`TT_PRODUCTION_GO`:** NO_GO

**Language:** English (this page) | [ZH](../zh-CN/08-governance-boundary.md)

---

## TTG is

- Governance + budget program asset (25T genesis, NO-MINT)
- Not travel order settlement (USDC default)

## Country pool / FeeRouterV2 (table 1-01 · 04)

- Platform fee 5% (500 bps) — governance only to change
- Active steward: 45% of platform fee to steward wallet; 55% to **ProjectPoolV2** `0x65714bbF2f3B8bB7E4c71F5D51C0bbe6869dAB68`
- No steward: 100% to ProjectPoolV2
- Public sale USDC → ProjectPoolV2 (never Legacy P4Cap / old pool `0x7B21…`)

## Governance

- Official PM/Vault delay: **12h** NEW SoloTimelock `0xF61880fe…`. PATH_A set PM.timelock and Vault.admin to NEW 12h.
- Phase1 OLD 48h SoloTimelock `0x99e43F…`: **LEGACY** (still 48h on-chain; not living Official delay)

## Not claimed

- RegionVault snapshot/claim end-state (83 target — not Official LIVE)
- Production GO
- Exchange listings

SSOT: table 1-01 in `09-contract-addresses.md` and root HTML dashboard. FeeRouterV2 living `0x2F3F4120…`.
