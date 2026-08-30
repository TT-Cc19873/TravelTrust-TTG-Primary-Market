# 治理币与资金池边界

**状态：** `READY_NOT_PUBLISHED` · `DEPLOYED_PENDING_CUTOVER` · **`TT_PRODUCTION_GO`:** NO_GO

**语言：** 中文（本页） · [English](../en/08-governance-boundary.md)

---

## TTG 是什么

- 治理与预算程序资产（创世 25T · 不可增发 NO-MINT）
- **不是**旅行订单默认结算币（订单默认 **USDC**）

## 国家资金池 / FeeRouterV2（表 1-01 · 04）

- 平台费 5%（500 bps）— 仅治理可改
- 有活跃主理人：平台费的 45% 至主理人钱包；55% 至 **ProjectPoolV2** `0x65714bbF2f3B8bB7E4c71F5D51C0bbe6869dAB68`
- 无主理人：100% 至 ProjectPoolV2
- 公售 USDC → ProjectPoolV2（**永不**进入 Legacy P4Cap / 旧池 `0x7B21…`）

## 治理

- Governor → SoloTimelock → 定时操作
- Official 一级市场 / Vault 定时操作延迟：**12h**（NEW SoloTimelock `0xF61880fe…`）。PATH_A 已把 PM.timelock 与 Vault.admin 切到 NEW 12h。
- Phase1 OLD 48h SoloTimelock `0x99e43F…`：**LEGACY**（链上仍是 48h，不是活 Official 延迟）

## 未宣称

- RegionVault 快照/领取终局（83 目标 — 非 Official LIVE）
- Production GO
- 交易所上币
