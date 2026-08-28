# 语言规范 · Language Policy

## 中文

| 目录 | 语言规则 |
|------|----------|
| `docs/zh-CN/` | **简体中文正文**；链上/合约专有名词可保留英文（Governor、Timelock、NO-MINT、USDC） |
| `docs/en/` | **纯英文正文**；不得出现中文段落 |
| `docs/zh-CN/01–07` | 技术中文（来自 github-official/zh） |
| `docs/zh-CN/08–19` | 独立中文稿（非英文粘贴） |
| `ops-narrative/` | **运营叙事副本**（官网发布说明）· **不是** 01–19 材料号 |
| README | `README.zh-CN.md` 中文 · `README.en.md` 英文 |

如发现混语，请在主仓库修复后重新同步：`python scripts/dev/sync-ttg-primary-market-satellite-repo.py --build --deploy --staging-push --push`

## English

| Path | Rule |
|------|------|
| `docs/zh-CN/` | Simplified Chinese body; English for on-chain proper nouns |
| `docs/en/` | English only — no Chinese paragraphs |
| `docs/zh-CN/01–07` | Technical Chinese from github-official/zh |
| `docs/zh-CN/08–19` | Dedicated Chinese drafts |
| `ops-narrative/` | Ops narrative copy of Official www Web3 release notes — **not** pack 01–19 |
| README | `README.zh-CN.md` CN · `README.en.md` EN |
