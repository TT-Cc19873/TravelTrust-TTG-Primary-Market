> **语言：** 中文技术文档（专有名词保留英文，如 Governor、Timelock、USDC）· [English](../en/01-primary-market.md)

# 一级市场

**上游：** Documentation Truth Baseline · Design Lock **DL_R1** · Whitepaper PASS  
**Mainnet：** 公售时间表已 pin 为 `V9_SHORT_WINDOW_FIVE_ROUND`（Timelock execute 2026-08-26）· 兑换窗口 **尚未对公众开放** · **≠** Fully Active · **≠** `TT_PRODUCTION_GO`

NEW Batch Primary Market + PublicSaleVault 执行 Norm 五批短窗口（合计约占 25T 的 **3.905%**）：

| Batch | Cap（TTG） | USDC / 1 TTG（6 decimals raw） | UTC 窗口 |
|-------|------------|--------------------------------|----------|
| 1 | 1.25B | 1 | 2026-10-15 → 2026-10-22（7 天） |
| 2 | 6.25B | 3 | 2026-11-12 → 2026-11-26（14 天） |
| 3 | 31.25B | 5 | 2027-01-12 → 2027-02-02（21 天） |
| 4 | 312.5B | 7 | 2027-03-09 → 2027-04-08（30 天） |
| 5 | 625B | 9 | 2027-05-06 → 2027-06-20（45 天） |

- 价格阶梯不变：`1 / 3 / 5 / 7 / 9` µUSDC per whole TTG（约 `$0.000001` → `$0.000009`）
- 轮次之间留空档（避开圣诞与春节）。窗口是 `[start, end)`。
- `pinSaleScheduleFromNorm` 已经过 NEW 12h Timelock **execute**；五批仍 **unarmed**。公布计划 **不等于** 现在可以买入。
- **公售 USDC → NEW ProjectPool** · 永远不是 Legacy P4Cap
- Market：`0xc714E2567982ea92d5f3C5b66ab65532Cfc5f09b` · Vault：`0xe87378e49Ead2E1a422B8cae118d3C905Ee45B6C`
