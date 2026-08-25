# Hermes Agent MCP 工具文档

**更新日期：** 2026-08-25  
**MCP 服务器：** research-assistant  
**状态：** ✓ 已启用（通过 hermes mcp list 确认）

---

## 工具列表

| # | 工具名 | 功能描述 |
|---|--------|----------|
| 1 | `check_health` | 检查 MCP Server 各组件状态：适配器可用性、编码器类型、期刊数据库条目数 |
| 2 | `index_and_search` | 从多个学术数据库并行抓取论文并建立语义索引，然后执行语义检索 |
| 3 | `search_papers` | 检索论文：优先语义检索，索引为空时自动回退多源并行搜索 |
| 4 | `search_by_id` | 根据 DOI / PMID / arXiv ID 精确查询单篇论文元数据 |
| 5 | `map_evidence` | 对论断检索相关文献并生成证据链，含强/弱/无三级强度标记 |
| 6 | `analyze_data` | 统计分析：t-test / ANOVA / Pearson 相关 / Spearman 相关 / 描述性统计 |
| 7 | `run_r_script` | 在 R 环境中执行 R 代码，返回 JSON 结果（需安装 R 和 rpy2） |
| 8 | `format_citation` | 格式化论文引用：支持 GB/T 7714 / APA / MLA / Chicago / IEEE / Harvard 6 种格式 |
| 9 | `generate_report` | 生成学术论文报告（Word .docx 或 LaTeX .tex），适配 Nature/Science/Cell 等 338 个期刊模板 |
| 10 | `list_journals` | 列出期刊模板数据库，支持按学科领域或关键词搜索（limit 最大 100） |
| 11 | `get_journal_spec` | 获取单个期刊的完整模板规格（LaTeX/Word 参数、引用格式、摘要字数限制等） |
| 12 | `check_update` | 检查学术助手是否有新版本可用，返回当前版本、远程最新版本 |
| 13 | `apply_update` | 执行自动更新：下载最新版本、备份旧版本、应用更新 |
| 14 | `fetch_journal_online` | 从 CrossRef API 实时查询期刊规格，输入 ISSN 或期刊名，返回最新排版参数 |
| 15 | `update_journal_database` | 从 CrossRef API 批量更新本地期刊数据库，支持期刊名或 ISSN 列表 |

---

## Resources

| URI | 说明 |
|-----|------|
| `journals://list` | 期刊数据库完整列表（JSON） |
| `journals://spec/{key}` | 单个期刊模板规格（JSON） |
| `citation://formats` | 支持的 6 种引用格式说明（JSON） |
| `evidence://rules` | 证据强度判定规则（JSON） |

---

## Prompts

| 名称 | 说明 |
|------|------|
| `literature_review` | 生成文献综述框架，基于给定研究主题检索相关论文并结构化输出 |
| `research_report` | 基于证据映射生成完整研究报告，含摘要、引言、方法、结果、讨论、结论 |

---

## MCP 配置信息

```yaml
research-assistant:
  command: /opt/research-assistant/.venv/bin/python
  args:
    - /opt/research-assistant/mcp_server.py
  env:
    SBERT_OFFLINE: "1"
    PYTHONPATH: /opt/research-assistant
```

> 文档由 Hermes Agent 自动生成 | 更新于 2026-08-25
