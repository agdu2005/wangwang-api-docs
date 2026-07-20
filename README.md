# WangWang Agent API 文档

> 更新日期：2026-07-20
> 
> 本文档由旺旺自动生成，记录所有已配置的 MCP 工具接口。

---

## 📊 MCP 服务状态总览

| 服务名称 | 状态 | 工具数 | 功能说明 |
|---------|------|--------|---------|
| antv-chart | ✅ | 123 | 金融市场数据（股票/基金/期货/宏观） |
| antv-visual | ✅ | 25 | ECharts 可视化图表生成 |
| bmi-mcp | ✅ | 1 | BMI 体重指数计算 |
| bw-ir | ✅ | 1 | 发票真实验证 |
| didi | ❌ | - | 滴滴打车（连接失败，接口不可用） |
| food-detective | ✅ | 1 | 美食推荐 |
| how-to-cook | ✅ | 5 | 菜谱查询与智能推荐 |
| luckin | ⛔ | - | 瑞幸咖啡（已禁用） |
| market-cmapi | ✅ | 2 | 中国地区新闻查询 |
| mbti | ⛔ | - | MBTI人格测试（已禁用） |
| openscad | ✅ | 7 | 3D建模与图片生成 |
| vision-mcp | ✅ | 1 | 图片内容分析 |
| gezhe | ✅ | 1 | PPT演示文稿生成 |
| playwright | ❌ | - | 浏览器自动化（连接失败） |
| pandoc | ✅ | 1 | 文档格式转换 |
| doc-forge | ✅ | 16 | 文档处理（PDF/HTML/Markdown等） |
| excel | ✅ | 6 | Excel 读取写入操作 |
| minimax | ❌ | - | MiniMax AI（超时） |
| mmb-mcp | ❌ | - | 慢慢买数据（认证失败） |
| qrcode-mcp | ✅ | 1 | 二维码生成 |
| stock-quote | ✅ | 21 | 全球股票/期货/外汇行情 |
| amap | ✅ | 12 | 高德地图（地理编码/路径规划/天气） |
| github | ✅ | 26 | GitHub 仓库/Issues/PR 管理 |
| sqlite | ✅ | 5 | SQLite 数据库操作 |
| weather | ✅ | 3 | 天气/预报/空气质量 |
| local_time | ✅ | 1 | 获取当前本地时间 |
| xhs-toolkit | ❌ | - | 小红书工具包（连接失败） |
| xhs-toolkit-http | ❌ | - | 小红书工具包HTTP（服务未启动） |
| gf-windmill | ⛔ | - | 广发Windmill（已禁用） |

**统计：共 29 个 MCP 服务，✅ 正常 18 个，❌ 失败 8 个，⛔ 禁用 3 个**

---

## 工具详情

---

### 1. antv-chart（金融市场数据）

**功能：** 沪深京A股、基金、期货、宏观经济数据查询

**工具数：** 123

| 工具名 | 功能说明 |
|--------|---------|
| list_stocks_dividends | 分红派息查询 |
| list_stock_offerings | 增发方案查询 |
| list_stocks_rights_issue_res | 配股发行结果 |
| list_stock_top10_circulating_shareh | 十大流通股东 |
| list_stock_capital_changes | 股本变动历史 |
| list_stock_freeze_details | 股权冻结明细 |
| list_stock_pledge_details | 股权质押明细 |
| list_stock_repurchase_plans | 股份回购计划 |
| list_stock_institutional_holdings_stats | 机构持股统计 |
| list_stock_tender_offers | 要约收购 |
| get_trade_special_date | 交易日衍生日期 |
| list_stk_income_state_pit | 利润表数据 |
| list_stk_balan_sheet_pit | 资产负债表数据 |
| list_stock_cash_flows_pit | 现金流量表数据 |
| list_fund_all | 全市场基金列表 |
| list_fund_hold_industry | 基金持仓行业 |
| list_index_quote_barch | 指数行情柱状图数据 |
| list_report_institutions | 研究机构列表 |
| list_stock_unadjusted_quotes | 未复权行情数据 |
| list_stock_share_adj_factors | 除权除息事件 |
| get_company_profiles | 公司基本信息 |
| list_index_quotes | 指数日行情数据 |
| list_stock_report_schema | 定期报告预披露日程 |
| list_stock_major_contracts | 重大合同公告 |
| get_stock_margin_securities | 融资融券标的证券 |
| list_stock_executive_shareholding_change | 高管持股变动 |
| get_cn_trade_calender_list | A股交易日列表 |
| list_stock_management_dirs | 管理层信息 |
| list_stock_core_mgmt_changes | 核心管理层变更 |
| list_stock_related_transactions | 关联交易详情 |
| list_industries | 行业列表 |
| get_stock_rights_issues | 配股发行信息 |
| list_concepts | 概念列表 |
| get_stock_basic_info | 股票基本信息 |
| list_stock_absorption_mergers | 吸收合并事件 |
| list_stock_earnings_bulletins | 业绩快报数据 |
| list_stock_cash_flows | 现金流量数据 |
| list_stock_income_statements | 利润详情 |
| list_stock_balance_sheet | 资产负债表 |
| list_stock_adjusted_quotes | 复权行情数据 |
| list_fund_daily_quotes | 基金日行情数据 |
| list_stock_special_notices | 特别提示信息 |
| list_fund_adj_quotes | 基金前复权日行情 |
| get_fund_code_assoc | 基金关联关系 |
| get_fund_basic_info | 基金基本信息 |
| get_fund_listings_record | 基金发行上市记录 |
| get_fund_categories | 基金分类体系 |
| get_fund_manager_basic_info | 基金经理基本信息 |
| list_stock_holder_cnt | 股东户数 |
| list_subscription_redemption_status | 基金申购赎回状态 |
| list_fund_invest_targets | 基金投资标的 |
| get_stock_former_names | 股票曾用名 |
| list_fund_perf_benchmarks | 基金业绩比较基准 |
| list_fund_fee_structures | 基金费率信息 |
| list_fund_award_records | 基金所获奖项 |
| get_stock_industries | 申万行业分类 |
| list_fund_nav_history | 基金历史净值 |
| list_currency_yield_history | 货币基金收益 |
| list_fund_adj_navs | 基金复权单位净值 |
| list_fund_return_rate | 基金历史回报率 |
| list_perf_benchmark_quote | 业绩比较基准行情 |
| list_fund_share_splits | 基金份额拆分折算 |
| list_fund_dividend_distributions | 基金分红信息 |
| list_hk_stock_dividends | 港股分红派息 |
| list_fund_portfolio_asset_holdings | 基金资产配置 |
| list_fund_portfolio_stock_holdings | 基金持仓股票 |
| generate_chart | ECharts图表转Base64图片 |
| list_fund_portfolio_bond_holdings | 基金持仓债券 |
| generate_nex_chart | 图表图片生成 |
| list_portfolio_fund_holdings | 基金持仓基金 |
| list_fund_shares | 基金份额变动 |
| list_fund_hold_structures | 基金持有人结构 |
| list_etf_constituent_stks | ETF成分股 |
| list_etf_sub_red_lists | ETF申购赎回清单 |
| list_fund_fin_inds_q | 基金季度财务指标 |
| list_fund_fin_inds | 基金主要财务指标 |
| list_economic_cn_cpi | 中国CPI数据 |
| list_economic_cn_ppi | 中国PPI数据 |
| list_industry_hold_fund | 行业持仓基金 |
| list_concept_hold_fund | 概念持仓基金 |
| is_trade_date | 判断是否为交易日 |
| get_index_basic_info | 指数基本信息 |
| search | 金融产品搜索 |
| list_stock_all | 全市场股票列表 |
| list_money_supplies | 货币供应量数据 |
| list_gover_bond_yield | 国债收益率曲线 |
| list_money_market_repo_in | 国债收益率数据 |
| list_social_financing_sto | 社会融资规模数据 |

---

### 2. antv-visual（可视化图表生成）

**功能：** 基于 ECharts 的各类图表图片生成

**工具数：** 25

| 工具名 | 功能说明 |
|--------|---------|
| generate_area_chart | 面积图，呈现连续数据的趋势变化 |
| generate_bar_chart | 水平条形图，用于比较数值数据 |
| generate_boxplot_chart | 箱线图，展示数据分布统计 |
| generate_column_chart | 柱状图，适合比较分类数据 |
| generate_district_map | 区域地图，展示地理分布 |
| generate_dual_axes_chart | 双轴图，组合不同量级数据 |
| generate_fishbone_diagram | 鱼骨图，因果分析 |
| generate_flow_diagram | 流程图，展示步骤与决策 |
| generate_funnel_chart | 漏斗图，展示转化流程 |
| generate_histogram_chart | 直方图，展示数据频率分布 |
| generate_line_chart | 折线图，展示时间趋势 |
| generate_liquid_chart | 水球图，单值可视化 |
| generate_mind_map | 思维导图，组织信息 |
| generate_network_graph | 网络图，展示关系网络 |
| generate_organization_chart | 组织架构图 |
| generate_path_map | 路线图，展示路径规划 |
| generate_pie_chart | 饼图，展示比例构成 |
| generate_pin_map | 点位图，展示地理位置 |
| generate_radar_chart | 雷达图，多维数据对比 |
| generate_sankey_chart | 桑基图，展示数据流向 |
| generate_scatter_chart | 散点图，展示数据关系 |
| generate_treemap_chart | 矩形树图，展示层级数据 |
| generate_venn_chart | 韦恩图，展示集合关系 |
| generate_violin_chart | 小提琴图，展示数据分布 |
| generate_word_cloud_chart | 词云图，展示词频权重 |

---

### 3. bmi-mcp（BMI体重指数）

**工具数：** 1

| 工具名 | 功能说明 |
|--------|---------|
| BMI体重指数 | 根据身高体重参数计算BMI，返回健康评估和健康建议 |

---

### 4. bw-ir（发票验证）

**工具数：** 1

| 工具名 | 功能说明 |
|--------|---------|
| invoice_verification | 验证发票的真实性和合规性，支持多种发票类型 |

---

### 5. food-detective（美食推荐）

**工具数：** 1

| 工具名 | 功能说明 |
|--------|---------|
| 推荐美食 | 传入地名，返回5条当地美食和推荐理由 |

---

### 6. how-to-cook（菜谱查询）

**工具数：** 5

| 工具名 | 功能说明 |
|--------|---------|
| mcp_howtocook_getAllRecipes | 获取所有菜谱 |
| mcp_howtocook_getRecipesByCategory | 根据分类查询菜谱（水产/早餐/调料/甜品/饮品/荤菜/素菜/汤/主食等） |
| mcp_howtocook_recommendMeals | 根据忌口、过敏原、人数智能推荐菜谱和购物清单 |
| mcp_howtocook_whatToEat | 不知道吃什么，根据人数推荐菜品组合 |
| mcp_howtocook_getRecipeById | 根据菜谱名称或ID查询完整详情 |

---

### 7. market-cmapi（新闻查询）

**工具数：** 2

| 工具名 | 功能说明 |
|--------|---------|
| 查询地区新闻 | 查询指定省市区的地方新闻 |
| 查询支持的新闻地区 | 查询API支持的省市区域列表 |

---

### 8. openscad（3D建模）

**工具数：** 7

| 工具名 | 功能说明 |
|--------|---------|
| create_3d_model | 根据自然语言描述创建3D模型 |
| modify_3d_model | 修改现有3D模型 |
| export_model | 导出3D模型为指定格式 |
| list_models | 列出所有已生成的3D模型 |
| generate_image | 使用Venice.ai生成图片 |
| generate_image_gemini | 使用Google Gemini生成图片 |
| get_supported_3d_shapes | 获取支持的3D形状类型 |

---

### 9. vision-mcp（图片分析）

**工具数：** 1

| 工具名 | 功能说明 |
|--------|---------|
| analyze_image | 分析图片内容并提供详细描述（基于Qwen3-VL-30B模型） |

---

### 10. gezhe（PPT生成）

**工具数：** 1

| 工具名 | 功能说明 |
|--------|---------|
| generate_ppt_by_topic | 根据主题生成PowerPoint演示文稿 |

---

### 11. pandoc（文档转换）

**工具数：** 1

| 工具名 | 功能说明 |
|--------|---------|
| convert-contents | 在不同文档格式间转换（Markdown/HTML/PDF/DOCX等） |

---

### 12. doc-forge（文档处理）

**工具数：** 16

| 工具名 | 功能说明 |
|--------|---------|
| document_reader | 读取文档文件内容 |
| pdf_merger | 合并多个PDF文件 |
| pdf_splitter | 拆分PDF文件 |
| docx_to_pdf | DOCX转PDF |
| docx_to_html | DOCX转HTML |
| html_cleaner | 清理HTML冗余标签 |
| html_to_text | HTML转纯文本 |
| html_to_markdown | HTML转Markdown |
| html_extract_resources | 提取HTML中的资源（图片/视频/链接） |
| html_formatter | 格式化HTML代码 |
| text_diff | 比较两个文本文件的差异 |
| text_splitter | 按分隔符或行数拆分文本 |
| text_formatter | 格式化文本缩进和间距 |
| text_encoding_converter | 文本编码转换 |
| excel_read | 读取Excel并转换为JSON |
| format_convert | 通用文档格式转换 |

---

### 13. excel（Excel操作）

**工具数：** 6

| 工具名 | 功能说明 |
|--------|---------|
| excel_copy_sheet | 复制工作表 |
| excel_create_table | 在工作表中创建表格 |
| excel_describe_sheets | 列出所有工作表信息 |
| excel_format_range | 格式化单元格区域 |
| excel_read_sheet | 分页读取工作表数据 |
| excel_write_to_sheet | 写入数据到工作表 |

---

### 14. qrcode-mcp（二维码生成）

**工具数：** 1

| 工具名 | 功能说明 |
|--------|---------|
| 二维码生成 | 生成二维码图片，存放在服务器上 |

---

### 15. stock-quote（股票行情）

**工具数：** 21

| 工具名 | 功能说明 |
|--------|---------|
| A股报价 | 沪深京A股实时报价 |
| A股K线 | A股K线数据 |
| A股K线复权 | 复权K线数据 |
| A股排行 | A股涨幅/跌幅/成交排行 |
| 港股报价 | 港股实时报价 |
| 港股K线 | 港股K线数据 |
| 港股排行 | 港股排行榜 |
| 美股报价 | 美股实时报价 |
| 美股K线 | 美股K线数据 |
| 美股排行 | 美股排行榜 |
| 美股品种 | 美股品种列表 |
| 内盘期货报价 | 国内期货实时报价 |
| 内盘期货K线 | 国内期货K线数据 |
| 内盘期货合约 | 国内期货合约信息 |
| 外盘期货报价 | 国外期货实时报价 |
| 外盘期货K线 | 国外期货K线数据 |
| 外盘期货合约 | 国外期货合约信息 |
| 全球指数报价 | 全球指数实时报价 |
| 全球指数K线 | 全球指数K线数据 |
| 外汇报价 | 外汇实时报价 |
| 外汇K线 | 外汇K线数据 |

---

### 16. amap（高德地图）

**工具数：** 12

| 工具名 | 功能说明 |
|--------|---------|
| maps_geo | 地址转经纬度坐标 |
| maps_regeocode | 经纬度转行政区划地址 |
| maps_ip_location | IP地址定位 |
| maps_weather | 城市天气预报 |
| maps_search_detail | POI详细信息查询 |
| maps_bicycling | 骑行路径规划（500km内） |
| maps_direction_walking | 步行路径规划（100km内） |
| maps_direction_driving | 驾车路径规划 |
| maps_direction_transit_integrated | 公交/地铁综合路径规划 |
| maps_distance | 两点间距离测量 |
| maps_text_search | 关键词POI搜索 |
| maps_around_search | 周边POI搜索 |

---

### 17. github（GitHub管理）

**工具数：** 26

| 工具名 | 功能说明 |
|--------|---------|
| search_repositories | 搜索GitHub仓库 |
| create_repository | 创建新仓库 |
| get_file_contents | 获取文件或目录内容 |
| create_or_update_file | 创建或更新文件 |
| push_files | 批量推送多个文件 |
| create_branch | 创建分支 |
| list_commits | 列出分支提交记录 |
| fork_repository | Fork仓库 |
| create_issue | 创建Issue |
| get_issue | 获取Issue详情 |
| list_issues | 列出仓库Issues |
| update_issue | 更新Issue |
| add_issue_comment | 添加Issue评论 |
| search_code | 搜索代码 |
| search_issues | 搜索Issues和PRs |
| search_users | 搜索用户 |
| create_pull_request | 创建Pull Request |
| get_pull_request | 获取PR详情 |
| list_pull_requests | 列出仓库PRs |
| create_pull_request_review | 创建PR Review |
| merge_pull_request | 合并PR |
| get_pull_request_files | 获取PR变更文件列表 |
| get_pull_request_status | 获取PR状态检查结果 |
| update_pull_request_branch | 更新PR分支 |
| get_pull_request_comments | 获取PR评论 |
| get_pull_request_reviews | 获取PR Reviews |

---

### 18. sqlite（数据库操作）

**工具数：** 5

| 工具名 | 功能说明 |
|--------|---------|
| list_tables | 列出所有表 |
| describe_table | 获取表结构信息 |
| read_query | 执行SELECT查询 |
| write_query | 执行INSERT/UPDATE/DELETE |
| create_table | 创建新表 |

---

### 19. weather（天气查询）

**工具数：** 3

| 工具名 | 功能说明 |
|--------|---------|
| get_weather | 获取当前天气（温度/湿度/风速/能见度） |
| get_forecast | 获取未来天气预报（最多3天） |
| get_air_quality | 获取空气质量指数 |

---

### 20. local_time（时间获取）

**工具数：** 1

| 工具名 | 功能说明 |
|--------|---------|
| get_current_time | 获取当前本地时间 |

---

## 📌 说明

- ❌ **失败**：服务已配置但连接超时或认证失败
- ⛔ **禁用**：在配置中明确设置为 disabled
- ✅ **正常**：服务可用，工具已发现

---
*文档由 WangWang Agent 自动生成 · 2026-07-20*
