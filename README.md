# 旺旺 API 文档

> 📅 更新日期：2026-08-28  
> 🤖 Hermès Gateway MCP 工具完整列表

---

## 📦 当前启用的 MCP 服务

### research-assistant（科研学术助手）

**功能描述**：多源文献检索、语义向量检索、统计分析、报告生成、证据映射。支持 DOI/PMID/arXiv ID 直接查询，338 个期刊模板（Nature/Science/Cell 等）。无网络时自动降级 TF-IDF + 内置样本数据。

**工具列表**：

| 工具名 | 功能说明 |
|--------|----------|
| `check_health` | 检查 MCP Server 各组件状态：适配器可用性、编码器类型、期刊数据库条目数 |
| `index_and_search` | 从多个学术数据库并行抓取论文并建立语义索引，然后执行语义检索 |
| `search_papers` | 检索论文：优先语义检索（需先index_and_search建立索引），索引为空时自动回退多源并行搜索 |
| `search_by_id` | 根据 DOI / PMID / arXiv ID 精确查询单篇论文元数据 |
| `map_evidence` | 对一条论断检索相关文献并生成证据链，含强/弱/无三级强度标记 |
| `analyze_data` | 统计分析：t-test / ANOVA / Pearson 相关 / Spearman 相关 / 描述性统计 |
| `run_r_script` | 在 R 环境中执行 R 代码，返回 JSON 结果（需安装 R 和 rpy2） |
| `format_citation` | 格式化论文引用：支持 GB/T 7714 / APA / MLA / Chicago / IEEE / Harvard 6 种格式 |
| `generate_report` | 生成学术论文报告（Word .docx 或 LaTeX .tex），适配 Nature/Science/Cell 等 338 个期刊模板 |
| `list_journals` | 列出期刊模板数据库，支持按学科领域或关键词搜索 |
| `get_journal_spec` | 获取单个期刊的完整模板规格（LaTeX/Word 参数、引用格式、摘要字数限制等） |
| `check_update` | 检查学术助手是否有新版本可用 |
| `apply_update` | 执行自动更新：下载最新版本、备份旧版本、应用更新 |
| `fetch_journal_online` | 从 CrossRef API 实时查询期刊规格（无需本地数据库） |
| `update_journal_database` | 从 CrossRef API 批量更新本地期刊数据库 |

---

## 📊 统计摘要

- **MCP 服务总数**：1
- **工具总数**：15
- **最后更新**：2026-08-28

---

*由旺旺自动生成*
