# 治理币与资金池边界

**状态：** `READY_NOT_PUBLISHED` · `DEPLOYED_PENDING_CUTOVER` · **`TT_PRODUCTION_GO`:** NO_GO

**语言：** 中文（本页） · [English](../en/08-governance-boundary.md)

---

## TTG 是什么

- 治理与预算程序资产（创世 25T · 不可增发 NO-MINT）
- **不是**旅行订单默认结算币（订单默认 **USDC**）

## 国家资金池 / FeeRouter

- 平台费 5%（500 bps）— 仅治理可改
- 有活跃主理人：平台费的 45% 至主理人钱包；55% 至 NEW ProjectPool
- 无主理人：100% 至 NEW ProjectPool
- 公售 USDC → NEW ProjectPool（**永不**进入 Legacy P4Cap）

## 治理

- Governor → SoloTimelock → 定时操作
- Phase1：OLD 48h Timelock 向 NEW 12h Timelock 迁移权限（PATH_A）

## 未宣称

- RegionVault 快照/领取终局（83 目标 — 非 Official LIVE）
- Production GO
- 交易所上币
