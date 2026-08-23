> **语言：** 中文技术文档（专有名词保留英文，如 Governor、Timelock、USDC）· [English](../en/02-governance.md)

# 治理

**上游：** Documentation Truth Baseline · Design Lock **DL_R1** · Whitepaper PASS  
**Mainnet：** `MAINNET_DEPLOYED_PHASE1` / `TIMELOCK_CUTOVER_PENDING` · **≠** Fully Active · **≠** `TT_PRODUCTION_GO`

```text
Governor → SoloTimelock（延迟 48h）
             admin = Marketing Norm 0xe1e732…
```

- **无 Safe** 作为 V9 Official Timelock admin
- 价格/批次/费率/payout 映射变更：仅治理路径
- Governance Burn：Governor → SoloTimelock → 授权 burner
- Phase1 Governor：`0xA0DfC4C5C544488AfEfE696AfB8e5823911e5A9c`
- Phase1 SoloTimelock：`0x99e43FaBA8dC773888223f70e1dfCd18bea37D7f`
- **Timelock 延迟：** 主网 Phase1 SoloTimelock = **48h**；Sepolia V9 外围排练 = **12h**（[Sepolia 部署](../deployments/sepolia.md)）— **勿混用**。
