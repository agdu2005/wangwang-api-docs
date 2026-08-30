# 🐶 旺旺 API 文档

**更新时间：2026-08-30 08:00 CST**

---

## MCP 工具列表

### ✅ 已启用

#### research-assistant（科研学术助手）
> 多源文献检索 · 统计分析 · 报告生成 · 证据映射 · 引用格式化

| 工具名称 | 功能说明 |
|---------|---------|
| `search_papers` | 语义检索已索引的论文数据库 |
| `search_by_id` | 根据 DOI / PMID / arXiv ID 精确查询单篇论文元数据 |
| `index_and_search` | 从多个学术数据库并行抓取论文并建立语义索引，然后执行检索 |
| `analyze_data` | 统计分析：t-test / ANOVA / Pearson 相关 / Spearman 相关 / 描述性统计 |
| `format_citation` | 格式化论文引用（GB/T 7714 / APA / MLA / Chicago / IEEE / Harvard） |
| `generate_report` | 生成学术论文报告（Word .docx 或 LaTeX .tex） |
| `list_journals` | 列出期刊模板数据库，支持搜索 |
| `get_journal_spec` | 获取单个期刊的完整模板规格 |
| `map_evidence` | Claim-Level 证据映射，论断 → 文献证据链 |
| `run_r_script` | 在 R 环境中执行 R 代码 |
| `check_health` | 检查 MCP Server 各组件状态 |

---

### 📦 可安装 MCP

| MCP 名称 | 功能描述 |
|---------|---------|
| `airtable` | Airtable 数据管理 |
| `asana` | Asana 任务管理 |
| `atlassian` | Jira + Confluence |
| `comfy-cloud` | 图片/视频/音频/3D 生成 |
| `datadog` | 日志/监控/仪表板 |
| `figma` | Figma 设计上下文 |
| `hugging_face` | Hugging Face 模型/数据集 |
| `intercom` | Intercom 对话/工单 |
| `linear` | Linear 问题追踪 |
| `n8n` | n8n 工作流管理 |
| `netlify` | Netlify 部署管理 |
| `notion` | Notion 页面和数据库 |
| `paypal` | PayPal 支付/发票 |
| `sentry` | Sentry 错误追踪 |
| `square` | Square 支付/目录 |
| `stripe` | Stripe 支付管理 |
| `supabase` | Supabase 数据库/认证/存储 |
| `unreal-engine` | Unreal Engine 5 编辑器 |
| `vercel` | Vercel 部署管理 |
| `webflow` | Webflow 网站/CMS |

---

**安装命令：** `hermes mcp install <name>`
