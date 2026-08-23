# 视频与媒体说明 · Video & Media Guide

**[中文](#中文)** | **[English](#english)**

---

## 中文

### 两种 MP4，不要混用

| 类型 | 文件 / 位置 | 用途 | 一级市场材料包 |
|------|-------------|------|----------------|
| **产品 Demo（标准）** | `docs/fundraising/external/export-ready/demo/TravelTrust-Product-Demo-v*.mp4` | 约 **90 秒一镜**：市场 → 下单 → Escrow → 争议/评分（见 SCREEN-RECORDING-BRIEF） | **首选**（投资人/LP、产品 BD 正式包） |
| **角色身份宣传片** | `frontend/public/media/traveltrust/roles/*.mp4` | `/traveltrust` 角色剧场：谁在用协议 | **可作补充**，不能冒充标准 Demo |

### 你们已有的 6 条角色视频（可用）

| 角色 | 文件 | 公开路径（官网部署后） |
|------|------|------------------------|
| 旅行者 | `traveler.mp4` | `/media/traveltrust/roles/traveler.mp4` |
| 向导 | `guide.mp4` | `/media/traveltrust/roles/guide.mp4` |
| 商家 | `merchant.mp4` | `/media/traveltrust/roles/merchant.mp4` |
| 服务商 | `provider.mp4` | 与 merchant 同源 |
| 旅行收购 | `acquisition.mp4` | `/media/traveltrust/roles/acquisition.mp4` |
| 区域主理人 | `region_steward.mp4` | `/media/traveltrust/roles/region_steward.mp4` |

**结论：可以用**，但请标注为 **「角色身份介绍 / 产品叙事补充」**，不要写成「已完成 90 秒产品全流程 Demo」。

### 推荐对外说法

- 有角色宣传片 → 证明**多身份产品叙事**已就绪  
- 仍建议补录 **90 秒产品路径录屏**（按 SCREEN-RECORDING-BRIEF）用于正式 BD / 部分平台材料  

### PDF（本仓库 `assets/pdf/`）

| 文件 | 说明 |
|------|------|
| `TTG-Primary-Market-OnePager-zh-CN.pdf` / `-en.pdf` | One Pager 文字版 |
| `TTG-Primary-Market-PitchDeck-outline-zh-CN.pdf` / `-en.pdf` | Pitch **内容大纲**（非视觉设计终稿） |

生成命令（主仓库）：

```bash
python scripts/dev/build-ttg-primary-market-pdf-pack.py
python scripts/dev/sync-ttg-primary-market-satellite-repo.py --build --deploy --staging-push --push
```

---

## English

### Two MP4 types — do not mix

| Type | Location | Purpose | Primary market pack |
|------|----------|---------|---------------------|
| **Product demo (canonical)** | `export-ready/demo/TravelTrust-Product-Demo-v*.mp4` | **~90s one-take**: market → order → escrow → dispute/rating | **Preferred** for LP / formal BD |
| **Role identity promos** | `frontend/public/media/traveltrust/roles/*.mp4` | `/traveltrust` theater — who uses the protocol | **Supplement only** — not a substitute for the canonical demo |

Six role videos exist (traveler, guide, merchant, provider, acquisition, region_steward). **Usable** as role-intro supplements; label honestly.

PDFs under `assets/pdf/` are text-based one-pager and pitch **outline** — not a designed visual deck.
