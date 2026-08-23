> **Language:** English (this page) · [中文](../zh-CN/02-governance.md)

# Governance

**Upstream:** Documentation Truth Baseline · Design Lock **DL_R1** · Whitepaper PASS  
**Mainnet:** `MAINNET_DEPLOYED_PHASE1` / `TIMELOCK_CUTOVER_PENDING` · **≠** Fully Active · **≠** `TT_PRODUCTION_GO`

```text
Governor → SoloTimelock (48h delay)
             admin = Marketing Norm 0xe1e732…
```

- **No Safe** as V9 Official Timelock admin
- Price/batch/fee-rate/payout-map changes: governance path only
- Governance Burn: Governor → SoloTimelock → authorized burner
- Phase1 Governor: `0xA0DfC4C5C544488AfEfE696AfB8e5823911e5A9c`
- Phase1 SoloTimelock: `0x99e43FaBA8dC773888223f70e1dfCd18bea37D7f`
- **Timelock delay:** Mainnet Phase1 SoloTimelock = **48h**; Sepolia V9 periphery rehearsal = **12h** ([Sepolia deployments](../deployments/sepolia.md)) — **do not conflate**.
