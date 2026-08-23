# 平台格式合规对照 · Platform Format Compliance

**[中文](#中文)** | **[English](#english)**

> 诚实评估：本仓库是 **披露材料 Markdown 包**，不是各平台可直接上传的成品文件集。  
> **Launchpad/交易所（CoinList、Binance 等）非本项目主轨**（无 KYC 冲突）。

---

## 中文

| 市场 / 平台 | 本项目轨道 | 平台通常要求的格式 | 本仓库现状 | 结论 |
|-------------|-----------|-------------------|------------|------|
| **M-00 链上五批公售** | PRIMARY | 链上 execute + 前端展示；非文件上传 | Markdown 参数说明 `01-primary-market` | **内容够披露** · 执行靠 Timelock cutover |
| **M-01 Etherscan** | PRIMARY | 网页表单 + Logo URL（32×32 活链）+ 英文描述 | `19-etherscan-pack` + `assets/etherscan/*.json` + SVG | **草稿就绪** · 缺网页提交 · 缺团队链接 |
| **M-02 GitHub Official** | PRIMARY | Markdown 文档树 | `01–07` 来自 github-official | **格式符合** · Wave2 待 Reality |
| **M-03 官网** | PRIMARY | HTML 页面（非本仓） | 仅 Markdown 草稿 | **内容参考** · 须 FE 发布 |
| **M-30 产品 BD** | PRODUCT | PDF/PPT One Pager + Demo 视频 | `15-one-pager` 仅 MD · 无 PDF/PPT/MP4 | **格式不足** · 缺视觉 Deck |
| **CoinList Passage** | N/A | 法人文件、KYC、法律意见、PDF 数据室 | 未准备 | **不适用** |
| **Binance/OKX/Bybit/Gate/KuCoin** | N/A | 上币/IEO 表单、审计 PDF、法律、KYC | 未准备 | **不适用** |
| **DAO Maker / Seedify** | N/A | 在线申请 + KYC + Deck PDF | 未准备 | **不适用** |
| **Fjord** | 暂缓 | 链上创建 sale + 合约参数 | 未按 Fjord 模型准备 | **未来单独立项** |

### 本仓库实际提供的文件格式

| 格式 | 有 | 无 |
|------|----|----|
| Markdown（`.md`） | ✅ 全部文档 | — |
| JSON（地址、Etherscan 草稿） | ✅ `assets/` | — |
| SVG/PNG Logo | ✅ `assets/brand/` | — |
| PDF One Pager / Pitch Deck | — | ❌ Owner 待做 |
| MP4 Demo | — | ❌ Owner 待录 |
| 平台专用表格/Typeform 导出 | — | ❌ 且多数平台 N/A |

### 语言规范

见 [LANGUAGE-POLICY.md](LANGUAGE-POLICY.md)。

---

## English

| Market / platform | Track | Typical required formats | This repo | Verdict |
|-------------------|-------|--------------------------|-----------|---------|
| **M-00 On-chain 5-batch sale** | PRIMARY | On-chain execute + UI; not file upload | Markdown params `01-primary-market` | **Disclosure OK** · execution = Timelock |
| **M-01 Etherscan** | PRIMARY | Web form + live 32×32 logo URL + EN description | `19-etherscan-pack` + JSON + SVG | **Draft ready** · not submitted · team links missing |
| **M-02 GitHub Official** | PRIMARY | Markdown tree | `01–07` from github-official | **Format OK** · Wave2 after Reality |
| **M-03 Website** | PRIMARY | HTML pages (not this repo) | Markdown drafts only | **Content ref** · needs FE publish |
| **M-30 Product BD** | PRODUCT | PDF/PPT one-pager + demo video | MD only | **Format gap** · no visual deck |
| **CoinList / CEX Launchpads** | N/A | Legal, KYC, audit PDF, data room | Not prepared | **NOT_APPLICABLE** |
| **Fjord** | Deferred | On-chain sale creation | Not prepared for Fjord model | **Future workstream** |

See [LANGUAGE-POLICY.md](LANGUAGE-POLICY.md).
