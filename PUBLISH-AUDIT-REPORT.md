# 发布审核报告 · Publish Audit Report

**Verdict:** `STOP_NOT_PUBLISH_READY`
**At UTC:** 2026-08-30T10:15:37Z

## 结论（诚实）

| 问题 | 答案 |
|------|------|
| 能否当 **Launchpad/交易所申请包** 外发？ | **否**（无 KYC 轨 + 多缺口） |
| 能否当 **GitHub 内部披露草稿**？ | **是**（Markdown + 重建 PDF） |
| 能否当 **一级市场链上披露** 文字真源？ | **部分**（M-00 内容够；执行靠 cutover） |
| 当前 PDF 是否视觉终稿？ | **否** — One Pager 为 Pandoc+LO 草稿；Pitch 仅为**大纲** |

## PDF 审核（已重建）

- 引擎：**Pandoc + LibreOffice**（替代旧 fpdf2 单页草稿）
- 每份含：**DRAFT 状态 + 免责声明**
- Pitch PDF：**DRAFT_OUTLINE_ONLY**，非 15 页视觉 Deck
- 仍缺：品牌色、Logo 页、页眉页脚 IR 规范（见 fundraising `35-IR-PDF-出版-QA`）

## 一级市场申请标准对照

| 市场 | 内容 | 格式 | 可提交？ |
|------|------|------|----------|
| M-00 链上五批 | ✅ | N/A（链上） | cutover 后 |
| M-01 Etherscan | 草稿 | 表单+Logo | ❌ 未提交 |
| M-02 GitHub | ✅ | MD | cutover 后 |
| M-03 官网 | 草稿 | HTML | ❌ |
| M-30 BD | 部分 | PDF 草稿+无 Demo | ❌ |
| Launchpads | N/A | — | **不适用** |

## 发现项

- **P1** `md` — docs\en\00-START-HERE.md: Chinese in English doc
- **P1** `ai_production` — M-30: missing or undersized V9 90s demo MP4
- **P1** `ai_production` — M-30: missing 15-page IR visual Pitch Deck (PPTX+PDF)
- **P1** `ai_production` — IR-PUBLICATION-QA-LATEST.json missing
- **P1** `primary_market` — M-01 Etherscan: gap — team links + web form submit
- **P1** `primary_market` — M-03 Website: gap — HTML publish
- **P0** `publish` — team template still MISSING_OWNER_INPUT — blocks external send

机读：`PUBLISH-AUDIT-LATEST.json` · 复检：`python scripts/dev/audit-ttg-primary-market-publish-gate.py`
