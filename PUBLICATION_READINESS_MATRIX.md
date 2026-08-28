# Publication Readiness Matrix · 发布就绪矩阵

**Stamp:** `V9_PRIMARY_MARKET_PUBLICATION_READINESS_MATRIX`
**Verdict:** `V9_PRIMARY_MARKET_MANUAL_PUBLICATION_CLASSIFICATION_PASS_STOP`
**At UTC:** 2026-08-28T12:04:41Z

## 合并结论（PASS_CONTENT_CLEAN + STOP_NOT_PUBLISH_READY）

| 审计 | Verdict | 含义 |
|------|---------|------|
| Content / security / legal | `PASS_CONTENT_CLEAN` | 措辞与 V9 pins 一致 |
| Publish gate | `STOP_NOT_PUBLISH_READY` | 整包外发仍 STOP（团队/媒体缺口） |
| AI 可修项 | **0** | 须归零才 PASS_STOP |
| Owner 阻塞 | **5** | 不得 AI 代填 |
| Reality 阻塞 | **1** | Mainnet cutover 后替换 |

## 四级清单（现在怎么做）

### 现在可公开（PUBLIC_READY）

- DOC-00 00-START-HERE
- DOC-01 01-primary-market
- DOC-02 02-governance
- DOC-03 03-tokenomics
- DOC-04 04-ttg-v9
- DOC-05 05-architecture
- DOC-07 07-security
- DOC-08 08-governance-boundary
- DOC-11 11-faq
- DOC-13 13-security-summary
- DOC-17 17-public-contact
- DOC-18 18-project-intro

### 须 Owner 审后外发（PUBLIC_AFTER_OWNER_REVIEW）

- DOC-06 06-mainnet-deployments
- DOC-09 09-contract-addresses
- DOC-10 10-litepaper
- DOC-12 12-disclaimer
- DOC-15 15-one-pager
- DOC-16 16-media-fact-sheet

### 仅内部（INTERNAL_ONLY）

- DOC-14 14-team

### Mainnet Reality 后再发（DEFERRED_UNTIL_MAINNET_REALITY）

- DOC-19 19-etherscan-pack

## 逐篇裁决

| ID | Slug | Tier | 可外发理由 / 阻塞 | Owner 必审 | Reality 后替换 |
|----|------|------|-------------------|------------|----------------|
| DOC-00 | `00-START-HERE` | `PUBLIC_READY` | 导航+三事实写死+免责声明；无融资承诺 | — | mainnet_status_label, production_go_line |
| DOC-01 | `01-primary-market` | `PUBLIC_READY` | 五批 cap/价格与 github-official 一致；明示 cutover pending | — | timelock_execute_status, sale_availability_wording |
| DOC-02 | `02-governance` | `PUBLIC_READY` | Governor→Timelock 路径与 V9 一致；无越权承诺 | — | old_tl_migration_status, new_tl_active_label |
| DOC-03 | `03-tokenomics` | `PUBLIC_READY` | 50/35/3/5/7 与 25T NO-MINT 与 pins 一致 | — | marketing_norm_wallet_publish_note |
| DOC-04 | `04-ttg-v9` | `PUBLIC_READY` | 治理币边界/USDC/NO-MINT 核心事实 | — | phase1_address_status_label |
| DOC-05 | `05-architecture` | `PUBLIC_READY` | NEW/KEEP/LEGACY 三分；无旧叙事冒充 Official | — | active_registry_label |
| DOC-06 | `06-mainnet-deployments` | `PUBLIC_AFTER_OWNER_REVIEW` | Phase1 简表可披露但易误读 OLD 为终局 | confirm_phase1_summary_ok_pre_cutover | full_new_stack_promotion, verified_links |
| DOC-07 | `07-security` | `PUBLIC_READY` | 安全模型与 audit-candidate≠外部审计 表述诚实 | — | third_party_audit_url_if_published |
| DOC-08 | `08-governance-boundary` | `PUBLIC_READY` | 500bps/45-55/USDC/ProjectPool 与 V9 一致 | — | regionvault_endstate_wording |
| DOC-09 | `09-contract-addresses` | `PUBLIC_AFTER_OWNER_REVIEW` | 全量 OLD/NEW 地址透明但 cutover 前敏感 | confirm_publish_full_address_map_pre_cutover | legacy_section_retire, etherscan_verify_links |
| DOC-10 | `10-litepaper` | `PUBLIC_AFTER_OWNER_REVIEW` | 摘要草稿；非完整 Litepaper PDF | legal_wording_signoff | published_litepaper_url |
| DOC-11 | `11-faq` | `PUBLIC_READY` | 诚实 FAQ；否定审计 PASS/公售开放 | — | sale_open_answer, audit_answer_if_report_published |
| DOC-12 | `12-disclaimer` | `PUBLIC_AFTER_OWNER_REVIEW` | 风险披露模板；外发前须 Owner/法务过目 | owner_legal_signoff | jurisdiction_specific_addenda |
| DOC-13 | `13-security-summary` | `PUBLIC_READY` | 明确无第三方审计 PASS 宣称 | — | third_party_audit_report_url |
| DOC-14 | `14-team` | `INTERNAL_ONLY` | MISSING_OWNER_INPUT_all_identity_fields | display_name, role, x_url, linkedin, bio_x5, official_x | website_team_page_publish |
| DOC-15 | `15-one-pager` | `PUBLIC_AFTER_OWNER_REVIEW` | 文字草稿可备查；PDF 为 DRAFT 非 IR 终稿 | owner_legal_signoff, press_use_approval | stage_banner, demo_env_label |
| DOC-16 | `16-media-fact-sheet` | `PUBLIC_AFTER_OWNER_REVIEW` | 媒体 boilerplate 诚实；外发前 Owner 确认 | press_contact_authorization, boilerplate_signoff | mainnet_status_line, go_line |
| DOC-17 | `17-public-contact` | `PUBLIC_READY` | traveltrust.ir@gmail.com 与 registry 一致 | — | support_routing_if_changed |
| DOC-18 | `18-project-intro` | `PUBLIC_READY` | 标准介绍；治理币+USDC 边界清晰 | — | — |
| DOC-19 | `19-etherscan-pack` | `DEFERRED_UNTIL_MAINNET_REALITY` | not_submitted; contract_verify_prerequisite | team_links_for_form, owner_web_submit | etherscan_verified_url, logo_live_url_check |

## 整包级别

- GitHub 披露草稿：`PUBLIC_AFTER_OWNER_REVIEW`
- 外发/申请包：`INTERNAL_ONLY`
- Launchpad/CEX：`INTERNAL_ONLY`

机读：`PUBLICATION_READINESS_MATRIX.json` · 复检：
`python scripts/dev/run-ttg-v9-primary-market-publication-classification.py --require-pass`

