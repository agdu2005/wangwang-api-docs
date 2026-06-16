# Hermes Agent MCP API 文档

> 📅 更新时间: 2026-06-16  
> 🤖 Hermes Agent 版本: 最新  
> 📊 总计: 30个MCP服务器, 约240+工具

---

## 📋 目录

1. [HTTP传输型MCP](#http传输型mcp)
   - [antv-chart 金融数据](#1-antv-chart-金融数据)
   - [stock-quote 股票行情](#2-stock-quote-股票行情)
   - [didi 滴滴出行](#3-didi-滴滴出行)
   - [bmi-mcp BMI指数](#4-bmi-mcp-bmi指数)
   - [qrcode-mcp 二维码](#5-qrcode-mcp-二维码)
   - [gezhe PPT生成](#6-gezhe-ppt生成)
2. [Stdio传输型MCP](#stdio传输型mcp)
   - [github GitHub操作](#1-github-github操作)
   - [amap 高德地图](#2-amap-高德地图)
   - [weather 天气查询](#3-weather-天气查询)
   - [sqlite 数据库](#4-sqlite-数据库)
   - [playwright 浏览器自动化](#5-playwright-浏览器自动化)
   - [how-to-cook 菜谱查询](#6-how-to-cook-菜谱查询)
   - [doc-forge 文档处理](#7-doc-forge-文档处理)
   - [market-cmapi 财联社新闻](#8-market-cmapi-财联社新闻)
   - [vision-mcp 视觉理解](#9-vision-mcp-视觉理解)
   - [xhs-toolkit 小红书](#10-xhs-toolkit-小红书)
   - [其他工具](#11-其他工具)

---

## HTTP传输型MCP

### 1. antv-chart (金融数据)

> 金融市场数据API，支持A股、基金、债券、宏观经济数据查询

**连接状态**: ✅ Connected  
**工具数量**: 124 个  
**传输方式**: streamable_http

#### 股票数据
| 工具名 | 功能 |
|--------|------|
| `list_stocks_public_offering_place` | 通过股票代码和公告日期范围查询沪深京A股或B股的公开增发或配售结果 |
| `list_stocks_dividends` | 通过股票代码和分红年度截止日期范围 |
| `list_stock_offerings` | 通过股票代码和公告日期范围查询沪深京股票的增发方案详情 |
| `list_stocks_rights_issue_res` | 通过股票代码和日期范围查询沪深京股票的配股发行结果 |
| `list_stock_top10_circulating_shareh` | 通过股票代码和日期范围（格式：yyyy-MM-dd）查询指定沪深京股票的历史十大 |
| `list_stock_capital_changes` | 通过股票代码和日期范围查询公司股本变动历史 |
| `list_stock_freeze_details` | 通过股票代码和公告日期范围查询沪深京股票的股权冻结明细 |
| `list_stock_pledge_details` | 根据股票代码和公告日期范围 |
| `list_stock_repurchase_plans` | 通过股票名称或回购计划首次公告日期范围 |
| `list_stock_institutional_holdings_stats` | 通过股票代码和日期范围查询沪深京股票的机构持股统计数据 |
| `list_stock_tender_offers` | 根据股票代码及信息发布日期范围 |
| `get_trade_special_date` | 根据指定交易日期 |
| `list_stk_income_state_pit` | 通过股票代码（可批量）查询指定沪深京股票的利润表（时点）数据 |
| `list_stk_balan_sheet_pit` | 通过股票代码查询指定沪深京股票的资产负债表数据 |
| `list_stock_cash_flows_pit` | 通过股票代码（单个或批量）查询沪深京股票的现金流量表数据 |
| `list_fund_all` | 获取全市场基金列表 |
| `list_stock_all` | 获取全市场A股和B股股票的基本信息列表 |
| `list_fund_hold_industry` | 支持通过单个行业代码或批量行业代码数组查询持有对应行业股票的基金列表 |
| `list_index_quote_barch` | 支持通过单个指数代码或多个指数代码列表 |
| `list_report_institutions` | 支持通过机构名称（模糊查询）进行筛选 |
| `list_stock_unadjusted_quotes` | 使用股票代码和时间范围查询股票的未复权行情数据 |
| `list_stock_share_adj_factors` | 通过股票代码和日期范围查询指定股票的历史除权除息事件详情 |
| `get_company_profiles` | 通过股票代码查询股票所属公司的基本信息 |
| `list_index_quotes` | 通过指数代码和日期范围查询指数的历史日行情数据 |
| `list_stock_report_schema` | 通过股票代码和日期范围查询沪深京股票的定期报告（如年报、季报）预披露日程 |
| `list_stock_major_contracts` | 根据股票代码和公告发布日期范围 |
| `get_stock_margin_securities` | 通过股票代码查询融资融券标的证券及担保证券信息 |
| `list_stock_executive_shareholding_change` | 通过股票代码和日期范围查询公司高管及相关人员持股变动明细 |
| `get_cn_trade_calender_list` | 返回指定周期内的A股市场交易日列表 |
| `list_stock_management_dirs` | 通过股票代码、任职状态、任职开始和结束日期等条件 |
| `list_stock_core_mgmt_changes` | 通过股票代码和任职起始日期范围查询上市公司核心管理层（如董事长、总经理）的历史变 |
| `list_stock_related_transactions` | 通过股票代码和日期范围查询上市公司关联交易的详细信息 |
| `list_industries` | 通过行业名称（支持模糊匹配）或行业类型（指定行业体系）查询行业列表 |
| `get_stock_rights_issues` | 根据股票代码和公告日期范围查询沪深京股票的配股发行信息 |
| `list_concepts` | 概念列表 |
| `list_stocks_dividends` | 通过股票代码和分红年度截止日期范围 |
| `list_stocks_public_offering_place` | 通过股票代码和公告日期范围查询沪深京A股或B股的公开增发或配售结果 |
| `get_stock_basic_info` | 使用股票代码查询沪深京市场A股、B股的详细基本信息 |
| `list_stocks_rights_issue_res` | 通过股票代码和日期范围查询沪深京股票的配股发行结果 |
| `list_stock_offerings` | 通过股票代码和公告日期范围查询沪深京股票的增发方案详情 |
| `list_stock_capital_changes` | 通过股票代码和日期范围查询公司股本变动历史 |
| `list_stock_top10_circulating_shareh` | 通过股票代码和日期范围（格式：yyyy-MM-dd）查询指定沪深京股票的历史十大 |
| `list_stock_pledge_details` | 根据股票代码和公告日期范围 |
| `list_stock_freeze_details` | 通过股票代码和公告日期范围查询沪深京股票的股权冻结明细 |
| `list_stock_absorption_mergers` | 通过股票代码和日期范围查询沪深京A股、B股公司的吸收合并事件详情 |
| `list_stock_repurchase_plans` | 通过股票名称或回购计划首次公告日期范围 |
| `list_stock_tender_offers` | 根据股票代码及信息发布日期范围 |
| `list_stock_earnings_bulletins` | 通过股票代码和日期范围查询沪深京股票的业绩快报数据 |
| `list_stock_cash_flows` | 通过股票代码查询沪深京股票的现金流量数据 |
| `list_stock_income_statements` | 通过股票代码查询指定股票的利润详情 |

> 共 124 个工具，完整列表见上方输出

---

### 2. stock-quote (股票行情)

> A股、港股、美股、期货、外汇行情数据

**连接状态**: ✅ Connected  
**工具数量**: 21 个  
**传输方式**: streamable_http

| 工具名 | 功能 |
|--------|------|
| `A股K线` | A股K线 |
| `美股品种` | 美股品种 |
| `港股报价` | 港股报价 |
| `内盘期货K线` | 内盘期货K线 |
| `外盘期货K线` | 外盘期货K线 |
| `港股排行` | 港股排行 |
| `全球指数报价` | 全球指数报价 |
| `外汇K线` | 外汇K线 |
| `内盘期货报价` | 内盘期货报价 |
| `美股K线` | 美股K线 |
| `外盘期货报价` | 外盘期货报价 |
| `A股报价` | A股报价 |
| `A股排行` | A股排行 |
| `港股K线` | 港股K线 |
| `A股K线复权` | A股K线复权 |
| `外盘期货合约` | 外盘期货合约 |
| `外汇报价` | 外汇报价 |
| `美股排行` | 美股排行 |
| `美股报价` | 美股报价 |
| `全球指数K线` | 全球指数K线 |
| `内盘期货合约` | 内盘期货合约 |

---

### 3. didi (滴滴出行)

> 滴滴出行服务：打车、路线规划、地点搜索

**连接状态**: ✅ Connected  
**工具数量**: 13 个  
**传输方式**: SSE

| 工具名 | 功能 |
|--------|------|
| `maps_direction_bicycling` | 根据用户输入的起点终点坐标 |
| `maps_direction_driving` | 根据用户起终点经纬度坐标规划以小客车、轿车通勤出行的方案 |
| `maps_direction_transit` | 根据用户起终点坐标 |
| `maps_direction_walking` | 根据用户输入的起点终点坐标 |
| `maps_place_around` | 根据用户传入关键词和位置坐标 |
| `maps_regeocode` | 将经纬度坐标转换为地址信息 |
| `maps_textsearch` | 根据用户传入关键词和城市 |
| `taxi_cancel_order` | 取消打车订单 |
| `taxi_create_order` | 直接通过API创建打车订单 |
| `taxi_estimate` | 查看当前可用的网约车车型 |
| `taxi_generate_ride_app_link` | 根据起点、终点和车型生成打开移动应用或小程序的深度链接 |
| `taxi_get_driver_location` | 获取打车订单对应司机的实时位置经纬度 |
| `taxi_query_order` | 查询打车订单的状态和信息 |

---

### 4. bmi-mcp (BMI指数)

> BMI体重指数计算与健康建议

**连接状态**: ✅ Connected  
**工具数量**: 1 个

| 工具名 | 功能 |
|--------|------|
| `BMI体重指数` | 根据身高、体重参数、查询BMI体重指数相关信息、返回BMI体重评估信息、健康提示信息、健康建议等。 |

---

### 5. qrcode-mcp (二维码)

> 二维码生成服务

**连接状态**: ✅ Connected  
**工具数量**: 1 个

| 工具名 | 功能 |
|--------|------|
| `二维码生成` | 二维码生成 图片存放在showapi服务器上,会不定期的清理,请及时拷贝!， |

---

### 6. gezhe (PPT生成)

> 根据主题生成PPT演示文稿

**连接状态**: ✅ Connected  
**工具数量**: 1 个

| 工具名 | 功能 |
|--------|------|
| `generate_ppt_by_topic` | Generate PowerPoint presentations from topics |

---

## Stdio传输型MCP

### 1. github (GitHub操作)

> GitHub仓库、PR、Issue管理

**连接状态**: ✅ Connected  
**工具数量**: 26 个  
**包**: @modelcontextprotocol/server-github

#### 搜索工具
| 工具名 | 功能 |
|--------|------|
| `search_repositories` | 搜索GitHub仓库 |
| `search_issues` | 搜索Issues和PRs |
| `search_code` | 搜索代码 |
| `search_users` | 搜索用户 |

#### 仓库操作
| 工具名 | 功能 |
|--------|------|
| `create_repository` | 创建新仓库 |
| `fork_repository` | Fork仓库 |
| `get_file_contents` | 获取文件/目录内容 |
| `create_or_update_file` | 创建或更新单文件 |
| `push_files` | 批量推送文件 |
| `list_commits` | 获取提交列表 |

#### Pull Request
| 工具名 | 功能 |
|--------|------|
| `create_pull_request` | 创建PR |
| `get_pull_request` | 获取PR详情 |
| `list_pull_requests` | 列出PRs |
| `merge_pull_request` | 合并PR |
| `get_pull_request_files` | 获取PR变更文件 |
| `get_pull_request_reviews` | 获取PR审查 |
| `create_pull_request_review` | 创建PR审查 |

#### Issue
| 工具名 | 功能 |
|--------|------|
| `create_issue` | 创建Issue |
| `get_issue` | 获取Issue详情 |
| `update_issue` | 更新Issue |
| `add_issue_comment` | 添加Issue评论 |
| `list_issues` | 列出Issues |

---

### 2. amap (高德地图)

> 高德地图服务：地理编码、路径规划、地点搜索

**连接状态**: ✅ Connected  
**工具数量**: 11 个  
**包**: @amap/amap-maps-mcp-server

| 工具名 | 功能 |
|--------|------|
| `maps_geo` | 地理编码 - 地址转经纬度 |
| `maps_regeocode` | 逆地理编码 - 经纬度转地址 |
| `maps_direction_driving` | 驾车路径规划 |
| `maps_direction_walking` | 步行路径规划 |
| `maps_direction_bicycling` | 骑行路径规划 |
| `maps_direction_transit_integrated` | 公交路径规划 |
| `maps_around_search` | 周边搜索 |
| `maps_text_search` | 关键词搜索POI |
| `maps_distance` | 距离测量 |
| `maps_weather` | 天气预报 |
| `maps_search_detail` | POI详情查询 |

---

### 3. weather (天气查询)

> 天气预报和空气质量

**连接状态**: ✅ Connected  
**工具数量**: 3 个

| 工具名 | 功能 |
|--------|------|
| `get_weather` | 获取当前天气 |
| `get_forecast` | 获取天气预报(1-5天) |
| `get_air_quality` | 获取空气质量 |

---

### 4. sqlite (数据库)

> SQLite数据库操作

**连接状态**: ✅ Connected  
**工具数量**: 5 个

| 工具名 | 功能 |
|--------|------|
| `list_tables` | 列出所有表 |
| `describe_table` | 获取表结构 |
| `read_query` | 执行SELECT查询 |
| `write_query` | 执行INSERT/UPDATE/DELETE |
| `create_table` | 创建新表 |

---

### 5. playwright (浏览器自动化)

> Playwright浏览器自动化控制

**连接状态**: ✅ Connected  
**工具数量**: 10 个

| 工具名 | 功能 |
|--------|------|
| `navigate` | 导航到URL |
| `screenshot` | 页面截图 |
| `click` | 点击元素 |
| `fill` | 填写表单字段 |
| `get_text` | 获取元素文本 |
| `wait_for_selector` | 等待元素出现 |
| `get_page_content` | 获取页面HTML |
| `close_browser` | 关闭浏览器 |
| `list_prompts` | 列出可用提示 |
| `get_prompt` | 获取指定提示 |

---

### 6. how-to-cook (菜谱查询)

> 中华菜谱数据库

**连接状态**: ✅ Connected  
**工具数量**: 5 个

| 工具名 | 功能 |
|--------|------|
| `get_all_recipes` | 获取所有菜谱 |
| `get_recipe_by_id` | 根据ID查询菜谱详情 |
| `get_recipes_by_category` | 按分类获取菜谱(水产/早餐/荤菜等) |
| `what_to_eat` | 根据人数推荐菜品 |
| `recommend_meals` | 智能推荐一周餐食计划 |

---

### 7. doc-forge (文档处理)

> 文档格式转换与处理

**连接状态**: ✅ Connected  
**工具数量**: 5 个

| 工具名 | 功能 |
|--------|------|
| `read` | 读取文档(PDF/DOCX/TXT/HTML/CSV) |
| `write` | 写入文档 |
| `merge` | 合并多个PDF |
| `split` | 分割PDF |
| `convert` | 格式转换(Markdown/HTML/PDF/DOCX) |

---

### 8. market-cmapi (财联社新闻)

> 财联社新闻与区域资讯

**连接状态**: ✅ Connected  
**工具数量**: 3 个

| 工具名 | 功能 |
|--------|------|
| `query_news` | 查询新闻 |
| `query_area_news` | 查询区域新闻 |
| `list_supported_areas` | 获取支持的省市列表 |

---

### 9. vision-mcp (视觉理解)

> 智谱GLM-4V图片分析

**连接状态**: ✅ Connected  
**工具数量**: 1 个

| 工具名 | 功能 |
|--------|------|
| `analyze_image` | 分析图片内容并提供详细描述 |

---

### 10. xhs-toolkit (小红书)

> 小红书内容运营工具

**连接状态**: ✅ Connected  
**工具数量**: 5 个

| 工具名 | 功能 |
|--------|------|
| `search_notes` | 搜索小红书笔记 |
| `get_note_detail` | 获取笔记详情 |
| `get_home_feed` | 获取首页推荐 |
| `xhs_search` | 小红书搜索(HTTP版) |
| `xhs_get_note` | 获取笔记(HTTP版) |

---

### 11. 其他工具

| MCP名称 | 功能描述 | 工具数 |
|---------|----------|--------|
| `bw-ir` | 发票真伪验证 | 1 |
| `food-detective` | 地方美食推荐 | 1 |
| `pandoc` | Pandoc文档转换 | 1 |
| `local_time` | 本地时间查询 | 1 |
| `mmb-mcp` | 谜语百科 | 2 |

---

## 📌 使用示例

### Python调用示例

```python
# 查股票行情
mcp_stock_quote_A___(
    market="hs_a",
    sort="changeRate",
    asc="0",
    page="1",
    limit="10"
)

# 查天气预报
mcp_weather_get_forecast(lat=22.543, lon=114.059, days=3)

# 生成二维码
mcp_qrcode_mcp______(
    content="https://example.com",
    size="6"
)

# 搜索GitHub仓库
mcp_github_search_repositories(
    query="stars:>1000 language:python"
)
```

---

*本文档由Hermes Agent自动生成*
