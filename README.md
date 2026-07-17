# Hermes Agent API 工具文档

> 🤖 Powered by Hermes Agent | 更新日期：2026年07月17日 08:03 CST

**⚠️ 状态说明** | 🟢 enabled = 已启用 | 🔴 disabled = 已禁用 | ⏳ available = 可用（未安装）

---

## 一、工具集总览（Built-in Toolsets）

| 状态 | 数量 | 工具集名称 |
|------|------|-----------|
| 🟢 enabled | 18 | web, browser, terminal, file, code_execution, vision, image_gen, tts, skills, todo, memory, session_search, clarify, delegation, cronjob, messaging, computer_use |
| 🔴 disabled | 9 | video, video_gen, x_search, moa, context_engine, homeassistant, spotify, yuanbao |

---

## 二、已启用工具集详情

### 1. web 🔍 Web Search & Scraping

网页搜索和内容抓取工具。

| 工具名称 | 功能说明 |
|---------|---------|
| `web_search` | 网络搜索，查询关键词相关信息 |
| `web_fetch` | 获取网页内容，支持 Markdown 格式提取 |

---

### 2. browser 🌐 Browser Automation

浏览器自动化控制。

| 工具名称 | 功能说明 |
|---------|---------|
| `browser_navigate` | 导航到指定 URL |
| `browser_snapshot` | 获取页面快照 |
| `browser_click` | 点击页面元素 |
| `browser_type` | 在输入框中输入文字 |
| `browser_scroll` | 滚动页面 |
| `browser_vision` | 截取页面截图 |

---

### 3. terminal 💻 Terminal & Processes

终端命令执行和进程管理。

| 工具名称 | 功能说明 |
|---------|---------|
| `terminal` | 执行 Shell 命令 |
| `process` | 管理后台进程 |

---

### 4. file 📁 File Operations

文件系统操作。

| 工具名称 | 功能说明 |
|---------|---------|
| `read_file` | 读取文件内容 |
| `write_file` | 写入文件内容 |
| `patch` | 补丁文件编辑 |
| `search_files` | 搜索文件内容 |
| `execute_code` | 执行 Python 代码 |

---

### 5. code_execution ⚡ Code Execution

Python 代码执行环境。

| 工具名称 | 功能说明 |
|---------|---------|
| `execute_code` | 执行 Python 代码，支持导入工具库 |

---

### 6. vision 👁️ Vision / Image Analysis

图像和视频内容分析。

| 工具名称 | 功能说明 |
|---------|---------|
| `vision_analyze` | 分析图片内容，提供详细描述 |

---

### 7. image_gen 🎨 Image Generation

AI 图像生成。

| 工具名称 | 功能说明 |
|---------|---------|
| `image_generate` | 根据文本提示生成图像 |

---

### 8. tts 🔊 Text-to-Speech

文本转语音。

| 工具名称 | 功能说明 |
|---------|---------|
| `text_to_speech` | 将文本转换为语音音频 |

---

### 9. skills 📚 Skills

技能管理。

| 工具名称 | 功能说明 |
|---------|---------|
| `skills_list` | 列出所有可用技能 |
| `skill_view` | 查看技能详情 |
| `skill_manage` | 管理技能（创建、更新、删除） |

---

### 10. todo 📋 Task Planning

任务规划管理。

| 工具名称 | 功能说明 |
|---------|---------|
| `todo` | 创建、更新、查看任务列表 |

---

### 11. memory 💾 Memory

持久化记忆存储。

| 工具名称 | 功能说明 |
|---------|---------|
| `memory` | 保存/读取持久化记忆 |

---

### 12. session_search 🔎 Session Search

会话历史搜索。

| 工具名称 | 功能说明 |
|---------|---------|
| `session_search` | 搜索历史会话内容 |

---

### 13. clarify ❓ Clarifying Questions

澄清问题。

| 工具名称 | 功能说明 |
|---------|---------|
| `clarify` | 向用户提问以澄清需求 |

---

### 14. delegation 👥 Task Delegation

任务委托。

| 工具名称 | 功能说明 |
|---------|---------|
| `delegate_task` | 委托子任务给其他 Agent |

---

### 15. cronjob ⏰ Cron Jobs

定时任务管理。

| 工具名称 | 功能说明 |
|---------|---------|
| `cronjob` | 创建、查看、删除定时任务 |

---

### 16. messaging 📨 Cross-Platform Messaging

跨平台消息发送。

| 工具名称 | 功能说明 |
|---------|---------|
| `send_message` | 向各平台发送消息 |

---

### 17. computer_use 🖱️ Computer Use (macOS)

macOS 电脑控制。

| 工具名称 | 功能说明 |
|---------|---------|
| `computer_use` | 控制 macOS 桌面应用 |

---

## 三、MCP 服务（Model Context Protocol）

### 已配置 MCP 服务器

当前无已配置的 MCP 服务器。

安装方式：`hermes mcp install <name>`

### 可用 MCP 目录

| 状态 | MCP名称 | 功能说明 |
|------|---------|---------|
| ⏳ available | linear | Find, create, and update Linear issues, projects, and comments |
| ⏳ available | n8n | Manage and inspect n8n workflows from Hermes |

### 安装已禁用工具

以下工具需要额外配置或服务支持：

| 工具集 | 状态 | 说明 |
|--------|------|------|
| video | 🔴 disabled | 视频分析功能 |
| video_gen | 🔴 disabled | 视频生成功能 |
| x_search | 🔴 disabled | X (Twitter) 搜索 |
| moa | 🔴 disabled | Mixture of Agents |
| context_engine | 🔴 disabled | 上下文引擎 |
| homeassistant | 🔴 disabled | Home Assistant 智能家居控制 |
| spotify | 🔴 disabled | Spotify 音乐控制 |
| yuanbao | 🔴 disabled | 腾讯元宝 |

---

## 四、已安装 Skills 列表

当前已安装 149 个技能（Skills），涵盖以下领域：

- 🚄 **出行**: 12306火车票查询、航班助手、酒店预订
- 🍜 **外卖**: 美团优惠券、饿了么订单
- 🛒 **购物**: 淘宝比价、京东返利
- 📊 **数据**: 金融数据、数据科学、Jupyter
- 🎨 **创意**: 图像生成、视频剪辑、PPT制作
- 📝 **文档**: PDF处理、Word/Excel/PPT
- 💬 **社交**: 微信自动化、小红书、X/Twitter
- 🏠 **办公**: Notion、Linear、Jira、飞书
- 🧠 **AI工具**: LLM调用、模型微调、推理服务
- 🔧 **开发**: GitHub、代码测试、Docker
- 🌤️ **生活**: 天气查询、跑腿服务、提醒

查看完整技能列表请访问：[skills](./skills/)

---

## 五、快速使用指南

### 1. 搜索网页
```
使用 web_search 工具搜索信息
```

### 2. 生成图片
```
使用 image_generate 工具，传入提示词
```

### 3. 操作文件
```
read_file 读取文件
write_file 写入文件
```

### 4. 执行代码
```
使用 execute_code 执行 Python 代码
```

### 5. 安装 MCP
```bash
hermes mcp install <mcp名称>
# 例如: hermes mcp install linear
```

---

> 📌 本文档由 Hermes Agent 自动生成
> 📅 更新日期：2026年07月17日 08:03 CST
> 🔗 仓库：https://github.com/agdu2005/wangwang-api-docs
