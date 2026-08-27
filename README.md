# Wangwang Agent API Docs

> 旺旺 Agent MCP & 工具集完整 API 文档  
> 更新时间：2026-08-27 08:01 (北京时间)

---

## 一、Built-in Toolsets（内置工具集）

| 工具集 | 功能描述 | 状态 |
|--------|---------|------|
| `web` | 🔍 Web 搜索与网页抓取 | ✓ enabled |
| `browser` | 🌐 浏览器自动化 | ✓ enabled |
| `terminal` | 💻 终端与进程管理 | ✓ enabled |
| `file` | 📁 文件操作（读/写/搜索/补丁） | ✓ enabled |
| `code_execution` | ⚡ Python 代码执行 | ✓ enabled |
| `vision` | 👁️ 视觉 / 图片分析 | ✓ enabled |
| `image_gen` | 🎨 AI 图片生成 | ✓ enabled |
| `bfl` | 🎬 BFL FLUX 3 视频生成 | ✓ enabled |
| `tts` | 🔊 文字转语音 | ✓ enabled |
| `skills` | 📚 Skills 技能管理 | ✓ enabled |
| `todo` | 📋 任务规划与追踪 | ✓ enabled |
| `memory` | 💾 记忆 / 上下文管理 | ✓ enabled |
| `session_search` | 🔎 会话历史搜索 | ✓ enabled |
| `clarify` | ❓ 澄清问题 | ✓ enabled |
| `delegation` | 👥 任务委托 / 子 Agent | ✓ enabled |
| `cronjob` | ⏰ 定时任务调度 | ✓ enabled |
| `computer_use` | 🖱️ 桌面自动化 (macOS/Windows/Linux) | ✓ enabled |

### 已禁用的工具集

| 工具集 | 功能描述 | 状态 |
|--------|---------|------|
| `video` | 🎬 视频分析 | ✗ disabled |
| `video_gen` | 🎬 视频生成 | ✗ disabled |
| `x_search` | 🐦 X (Twitter) 搜索 | ✗ disabled |
| `stt` | 🎙️ 语音转文字 | ✗ disabled |
| `homeassistant` | 🏠 Home Assistant | ✗ disabled |
| `spotify` | 🎵 Spotify | ✗ disabled |
| `yuanbao` | 🤖 腾讯元宝 | ✗ disabled |
| `context_engine` | 🧩 上下文引擎 | ✗ disabled |

---

## 二、MCP Servers（MCP 服务）

### research-assistant（科研学术助手）

**路径**: `/opt/research-assistant/`  
**Transport**: stdio  
**状态**: ✓ enabled

#### 工具列表

| 工具名 | 功能描述 |
|--------|---------|
| `search_papers` | 学术论文搜索（支持多源） |
| `search_by_id` | 按论文 ID / DOI 精确搜索 |
| `index_and_search` | 主题索引 + 语义搜索 |
| `map_evidence` | 证据映射，验证陈述真实性 |
| `analyze_data` | 统计分析（t-test / ANOVA / 相关性） |
| `run_r_script` | 执行 R 脚本进行数据分析 |
| `format_citation` | 格式化参考文献（多格式） |
| `generate_report` | 生成完整研究报告 |
| `list_journals` | 列出可用期刊及影响因子 |
| `get_journal_spec` | 获取目标期刊投稿规范 |
| `fetch_journal_online` | 在线获取期刊元数据 |
| `update_journal_database` | 更新期刊数据库 |
| `check_update` | 检查研究助手更新 |
| `apply_update` | 应用更新 |
| `literature_review_prompt` | 生成文献综述提示词 |
| `research_report_prompt` | 生成研究报告提示词模板 |

---

## 三、快速参考

### 常用命令

```bash
# 查看所有工具状态
hermes tools list

# 查看 MCP 服务状态
hermes mcp list

# 测试 MCP 连接
hermes mcp test <server_name>

# 列出所有可用 MCP 插件
hermes mcp catalog

# 安装新 MCP
hermes mcp install <name>
```

### MCP 插件生态（可安装）

| MCP | 功能描述 |
|-----|---------|
| `airtable` | Airtable 数据库操作 |
| `asana` | Asana 任务管理 |
| `figma` | Figma 设计上下文 |
| `hugging_face` | Hugging Face 模型/数据集 |
| `linear` | Linear 敏捷项目管理 |
| `notion` | Notion 笔记与数据库 |
| `stripe` | Stripe 支付集成 |
| `supabase` | Supabase 数据库/存储 |
| `vercel` | Vercel 部署管理 |
| `sentry` | Sentry 错误监控 |

---

*本文档由 旺旺 Agent 自动生成 | Hermès Agent MCP Inspector*
