> **语言：** 中文技术文档（专有名词保留英文，如 Governor、Timelock、USDC）· [English](../en/05-architecture.md)

# 架构

**上游：** Documentation Truth Baseline · `V9_DOCUMENTATION_FULL_CONVERGENCE_PASS` · `TTG_V9_MAINNET_EDITION_WHITEPAPER_PASS` · Design Lock **DL_R1**  
**Mainnet：** `MAINNET_DEPLOYED_PHASE1` / `TIMELOCK_CUTOVER_PENDING` · **≠** Fully Active · **≠** `TT_PRODUCTION_GO`

TravelTrust Web3 Mainnet Edition 采用 **NEW / KEEP / LEGACY** 三分：

| 类别 | 含义 |
|------|------|
| **NEW** | 表 1-01 活机：治理币、投票机、12 小时门、FeeRouterV2、ProjectPoolV2、柜台、币库、席位 |
| **KEEP** | 开单工厂 + 放款车间 + USDC（用户本金） |
| **LEGACY** | Safe / 旧 48h Timelock / P4Cap / Phase1 旧池·旧分账·旧 Governor·旧席位 / V8 / Remint — **不入** 表 1-01 |

```text
订单(+ISO 国家) → KEEP 工厂 / 放款车间
  → 平台费 5% → FeeRouterV2（表 1-01 · 04）
       ├─ 有主理人 → 45% 席位收款钱包 / 55% ProjectPoolV2
       └─ 无主理人 → 100% ProjectPoolV2
公售 USDC → ProjectPoolV2 `0x65714…`（永远不是 Legacy P4Cap / 旧池 `0x7B21…`）
投票机 `0xD4b616…` → 12 小时门 `0xF618…` → 外围运维 / Governance Burn
  （Phase1 OLD 48h SoloTimelock = LEGACY）
```

Token 货币规则 **NO-MINT 不可增发**。外围可经治理升级，**不得**借升级绕过 NO-MINT。
