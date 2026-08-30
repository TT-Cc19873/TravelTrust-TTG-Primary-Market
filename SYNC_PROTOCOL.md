# 同步协议 · Sync Protocol

**卫星仓库 Satellite:** [https://github.com/TT-Cc19873/TravelTrust-TTG-Primary-Market](https://github.com/TT-Cc19873/TravelTrust-TTG-Primary-Market)  
**主仓库 Monorepo:** `TravelTrust-V1.1`（私有工作仓）

---

## 中文

### 何时同步

主仓库更新以下任一内容后，应重新同步本卫星仓库：

1. `evidence/GO_ttg_v9_external_materials_closure/packages/`
2. `docs/github-official/zh/` 或 `docs/github-official/en/`
3. 一级市场矩阵 / 治理币披露字段
4. 官网发布说明文案（`frontend/locales` `traveltrust_unlock_*` · `docs/github-official/RELEASE-NOTES.md` · `web3-release-dashboard.html`）→ 卫星根目录 `TravelTrust-Web3-发布说明.html` / `.md`

### 命令（在主仓库根目录）

```bash
# 1. 刷新材料母版
python scripts/dev/run-ttg-v9-external-materials-closure.py --write-packages

# 2. 构建卫星仓库目录
python scripts/dev/sync-ttg-primary-market-satellite-repo.py --build

# 3. 部署到本地 clone 并推送（需已 clone 卫星仓库）
python scripts/dev/sync-ttg-primary-market-satellite-repo.py --build --deploy --push
```

环境变量（可选）：

- `TTG_PRIMARY_MARKET_REPO_DIR` — 本地卫星仓库路径（默认：与主仓库同级的 `TravelTrust-TTG-Primary-Market`）

### 纪律

- **禁止**在卫星仓库直接改母版正文（会被下次同步覆盖）
- **禁止**宣称 Production GO 或公售已开放（除非 Mainnet Reality PASS 后 Owner 书面授权）
- 改稿请回主仓库 → 跑同步脚本 → 再 push

---

## English

### When to sync

Re-sync this satellite repo after updating in the monorepo:

1. External materials packages under `evidence/GO_ttg_v9_external_materials_closure/packages/`
2. `docs/github-official/{zh,en}/`
3. Primary market matrix / governance disclosure fields
4. Official www Web3 release copy (`frontend/locales` `traveltrust_unlock_*` · `docs/github-official/RELEASE-NOTES.md` · `web3-release-dashboard.html`) → satellite root `TravelTrust-Web3-发布说明.html` / `.md`

### Commands (monorepo root)

Same as Chinese section above.

### Rules

- Do **not** edit canonical bodies in this repo (overwritten on next sync)
- Do **not** claim Production GO or open sale without Owner-authorized Reality PASS
- Edit in monorepo → run sync → push

---

**Matrix hub (monorepo):** `docs/fundraising/internal/24-一级市场矩阵体系-V9.md`
