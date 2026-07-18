# Hermes Agent API 文档

> 🤖 Powered by Hermes Agent | 更新日期：2026年07月18日 08:04 CST
> 
> ⚠️ 当前无已配置的 MCP 服务（hermes mcp list 返回空）
> 可安装 MCP：linear（Linear项目）、n8n（工作流）

---

## MCP 服务状态

| 状态 | 数量 | 说明 |
|------|------|------|
| 🟢 已启用 | 0 | 当前无已配置 MCP |
| 🔴 可用（未安装） | 2 | linear、n8n |

### 可安装 MCP

| MCP名称 | 状态 | 描述 |
|---------|------|------|
| linear | available | Find, create, and update Linear issues, projects, and comments |
| n8n | available | Manage and inspect n8n workflows from Hermes |

> 安装命令：`hermes mcp install <name>`

---

## 内置工具集（18个已启用 / 7个已禁用）

| 状态 | 工具集 | 说明 |
|------|--------|------|
| ✓ enabled | web | 🔍 Web Search & Scraping |
| ✓ enabled | browser | 🌐 Browser Automation |
| ✓ enabled | terminal | 💻 Terminal & Processes |
| ✓ enabled | file | 📁 File Operations |
| ✓ enabled | code_execution | ⚡ Code Execution |
| ✓ enabled | vision | 👁️ Vision / Image Analysis |
| ✗ disabled | video | 🎬 Video Analysis |
| ✓ enabled | image_gen | 🎨 Image Generation |
| ✗ disabled | video_gen | 🎬 Video Generation |
| ✗ disabled | x_search | 🐦 X (Twitter) Search |
| ✗ disabled | moa | 🧠 Mixture of Agents |
| ✓ enabled | tts | 🔊 Text-to-Speech |
| ✓ enabled | skills | 📚 Skills |
| ✓ enabled | todo | 📋 Task Planning |
| ✓ enabled | memory | 💾 Memory |
| ✗ disabled | context_engine | 🧩 Context Engine |
| ✓ enabled | session_search | 🔎 Session Search |
| ✓ enabled | clarify | ❓ Clarifying Questions |
| ✓ enabled | delegation | 👥 Task Delegation |
| ✓ enabled | cronjob | ⏰ Cron Jobs |
| ✓ enabled | messaging | 📨 Cross-Platform Messaging |
| ✗ disabled | homeassistant | 🏠 Home Assistant |
| ✗ disabled | spotify | 🎵 Spotify |
| ✗ disabled | yuanbao | 🤖 Yuanbao |
| ✓ enabled | computer_use | 🖱️ Computer Use (macOS) |

---

## 内置工具详情

### web（Web Search & Scraping）
- `web_extract_tool` — 网页内容提取
- `web_search_tool` — 搜索引擎搜索

### browser（Browser Automation）
- `browser_navigate` — 导航到URL
- `browser_snapshot` — 获取页面快照
- `browser_click` — 点击元素
- `browser_type` — 输入文本
- `browser_scroll` — 滚动页面
- `browser_vision` — 页面截图视觉分析
- `browser_back` — 返回上一页
- `browser_press` — 按键操作
- `browser_console` — 获取控制台输出
- `browser_get_images` — 获取页面图片列表

### terminal（Terminal & Processes）
- `terminal_tool` — 执行Shell命令

### code_execution（Code Execution）
- `execute_code` — Python代码执行

### vision（Vision / Image Analysis）
- `vision_analyze_tool` — 图像/视频分析
- `video_analyze_tool` — 视频分析

### image_gen（Image Generation）
- `image_generate_tool` — AI图片生成

### tts（Text-to-Speech）
- `text_to_speech_tool` — 文字转语音（微信禁用）

### skills（Skills Management）
- `skills_list` — 列出所有技能
- `skill_view` — 查看技能详情
- `skill_manage` — 创建/编辑/删除技能

### todo（Task Planning）
- `todo` — 任务清单管理

### memory（Memory）
- `memory` — 持久记忆存取

### session_search（Session Search）
- `session_search` — 跨会话历史搜索

### clarify（Clarifying Questions）
- `clarify_tool` — 生成澄清问题

### delegation（Task Delegation）
- `delegate_task` — 任务委托子代理

### cronjob（Cron Jobs）
- `cronjob_tools` — 定时任务管理

### messaging（Cross-Platform Messaging）
- `send_message_tool` — 跨平台发送消息

### computer_use（Computer Use - macOS）
- `handle_computer_use` — macOS自动化

### file（File Operations）
- `read_file` — 读取文件
- `write_file` — 写入文件
- `patch` — 局部编辑
- `search_files` — 搜索文件内容

### mcp（MCP Server Management）
- `mcp_tool` — MCP服务器管理

---

## 已安装 Skills（173个）

| 类别 | 数量 | 代表技能 |
|------|------|---------|
| 自动化 | 多 | browser-act, playwright, firecrawl, agent-reach |
| 开发 | 多 | github, git-commit, prisma-cli, python-design-patterns |
| 创意/设计 | 多 | frontend-design, shadcn-ui, excalidraw-diagram-generator |
| 数据 | 多 | jupyter-live-kernel, dataverse, cn-financial-scraper |
| 文档 | 多 | docx, pdf, pptx, word-docx, excel-xlsx |
| 办公协作 | 多 | notion-api, feishu, slack-workflows, jira-automation |
| 媒体 | 多 | youtube-content, spotify, gif-search |
| 社交 | 多 | twitter, xiaohongshu, discord-bot |
| AI/ML | 多 | openai, claude-api, huggingface-hub, llama-cpp |
| 生活服务 | 多 | flight-assistant, hotel-booking-ai, uupt-delivery |
| 专业工具 | 多 | valuation-analysis, westock-data, tavily-search-pro |

---

> 📌 本文档由 Hermes Agent 自动生成 | 每周定时更新
> 数据来源：`hermes mcp list` + `hermes tools list` + `hermes mcp catalog`
> GitHub仓库：agdu2005/wangwang-api-docs
