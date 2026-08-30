> **Language:** English (this page) | [ZH](../zh-CN/05-architecture.md)

# Architecture

**Upstream:** Documentation Truth Baseline · `V9_DOCUMENTATION_FULL_CONVERGENCE_PASS` · `TTG_V9_MAINNET_EDITION_WHITEPAPER_PASS` · Design Lock **DL_R1**  
**Mainnet:** `MAINNET_DEPLOYED_PHASE1` / `TIMELOCK_CUTOVER_PENDING` · **≠** Fully Active · **≠** `TT_PRODUCTION_GO`

TravelTrust Web3 Mainnet Edition uses a **NEW / KEEP / LEGACY** split:

| Class | Meaning |
|-------|---------|
| **NEW** | Table 1-01 living: token, Governor, 12h Timelock, FeeRouterV2, ProjectPoolV2, market, vault, RoleStake |
| **KEEP** | Escrow factory + SettlementRouter + USDC (user principal) |
| **LEGACY** | Safe / old 48h Timelock / P4Cap / Phase1 old pool·router·Governor·stake / V8 / Remint — **not** table 1-01 |

```text
Order(+ISO country) → KEEP factory / SettlementRouter
  → fee 5% → FeeRouterV2 (table 1-01 #04)
       ├─ Active steward → 45% payout wallet / 55% ProjectPoolV2
       └─ none → 100% ProjectPoolV2
Primary sale USDC → ProjectPoolV2 `0x65714…` (never Legacy P4Cap / old pool `0x7B21…`)
Governor `0xD4b616…` → 12h Timelock `0xF618…` → periphery ops / Governance Burn
  (Phase1 OLD 48h SoloTimelock = LEGACY)
```

Token monetary rules are **immutable NO-MINT**. Periphery may upgrade via governance **without** minting beyond genesis.
