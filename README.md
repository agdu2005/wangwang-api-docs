# 旺旺 API 文档

> 更新时间：2026-08-29 09:10:31 (北京时间 CST)

## MCP 工具总览

| 工具名称 | 功能描述 |
|---------|---------|
| **research-assistant** | 科研学术助手 MCP Server |

---

## research-assistant

科研学术助手：多源文献检索 · 语义向量检索 · 统计分析 · 报告生成 · 证据映射

**状态：** ✓ enabled (需要 MCP Python SDK)

### 工具列表

| 工具名 | 功能说明 |
|-------|---------|
| `search_papers` | 语义检索已索引的论文数据库 |
| `search_by_id` | 根据 DOI / PMID / arXiv ID 精确查询单篇论文元数据 |
| `index_and_search` | 从多个学术数据库并行抓取论文并建立语义索引，然后执行检索 |
| `analyze_data` | 统计分析：t-test / ANOVA / Pearson 相关 / Spearman 相关 / 描述性统计 |
| `format_citation` | 格式化论文引用（6 种格式：GB/T 7714 / APA / MLA / Chicago / IEEE / Harvard） |
| `generate_report` | 生成学术论文报告（Word .docx 或 LaTeX .tex） |
| `list_journals` | 列出期刊模板数据库，支持搜索 |
| `get_journal_spec` | 获取单个期刊的完整模板规格（如 nature / science / cell） |
| `map_evidence` | Claim-Level 证据映射，论断 → 文献证据链 |
| `run_r_script` | 在 R 环境中执行 R 代码 |
| `check_health` | 检查 MCP Server 各组件状态 |

---

## 可用 MCP 服务（未安装）

以下服务已注册但未启用，可通过 `hermes mcp install <name>` 安装：

| 服务名 | 功能 |
|-------|------|
| airtable | Airtable 数据库操作 |
| asana | Asana 任务管理 |
| atlassian | Jira + Confluence |
| comfy-cloud | Comfy 云端生图/视频/音频 |
| datadog | Datadog 监控 |
| figma | Figma 设计 |
| hugging_face | Hugging Face 模型/数据集 |
| intercom | Intercom 客服 |
| linear | Linear 项目管理 |
| n8n | n8n 工作流 |
| netlify | Netlify 部署 |
| notion | Notion 笔记 |
| paypal | PayPal 支付 |
| sentry | Sentry 错误追踪 |
| square | Square 支付 |
| stripe | Stripe 支付 |
| supabase | Supabase 数据库 |
| unreal-engine | Unreal Engine 5 |
| vercel | Vercel 部署 |
| webflow | Webflow CMS |

---

*由旺旺自动生成*
