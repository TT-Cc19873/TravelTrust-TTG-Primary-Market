# 安全与审计摘要

**状态：** `READY_NOT_PUBLISHED` · `DEPLOYED_PENDING_CUTOVER` · **`TT_PRODUCTION_GO`:** NO_GO

**语言：** 中文（本页） · [English](../en/13-security-summary.md)

---

## 安全模型（V9）

- TTG：NO-MINT；无公开持有人销毁；治理销毁经 Timelock
- 费用路由：Timelock 写入出款；基准 5%
- 资金池：90 天运营上限 ≤ 30% bps
- SoloTimelock 延迟：Official PM/Vault = **NEW 12h**；OLD 48h = **LEGACY**（PATH_A 之后）

## 审计状态

| 项 | 状态 |
|----|------|
| 内部 AI 审计波次（V9 candidate） | 仓库有证据 — **≠** 外部机构审计 |
| 第三方审计报告（公开） | **未发布** — 禁止宣称 |
| Bug bounty | 见公开 GitHub SECURITY.md |

漏洞报告：docs/github-official/SECURITY.md
