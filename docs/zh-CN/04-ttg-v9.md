> **语言：** 中文技术文档（专有名词保留英文，如 Governor、Timelock、USDC）· [English](../en/04-ttg-v9.md)

# TTG V9

**上游：** Documentation Truth Baseline · Design Lock **DL_R1** · Whitepaper PASS  
**Mainnet：** `MAINNET_DEPLOYED_PHASE1` / `TIMELOCK_CUTOVER_PENDING` · **≠** Fully Active · **≠** `TT_PRODUCTION_GO`

- Genesis 总量：**25,000,000,000,000 TTG（25T）**
- Genesis 后 **NO-MINT**（不可再增发）
- 供给仅可通过 **Governance Burn** 减少（Governor → SoloTimelock → 授权 burner）
- 非代理 Token；货币不变量硬编码
- Phase1 地址：`0xD5c1Ef9ec730F93e324A1966bD414a7f5ebc41c9` · 状态 `DEPLOYED_PENDING_CUTOVER`
- TTG **不是**旅行订单默认结算资产（本金为 USDC）
