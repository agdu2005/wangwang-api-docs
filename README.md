# Hermes Agent MCP API 文档

> 📅 更新时间: 2026年06月18日 08:09
> 🤖 Hermes Agent 版本: 最新
> 📊 总计: 28个MCP服务器（含23个已连接）

---

## 📋 目录

1. [已连接MCP列表](#已连接mcp列表)
2. [未连接/已禁用MCP](#未连接已禁用mcp)

---

## 已连接MCP列表

---

### 1. antv-chart（金融数据）

**功能**: A股/基金/指数/期货的金融数据查询与分析，支持124个工具

| 工具名称 | 功能说明 |
|---------|---------|
| list_stock_all | 获取全市场A股/B股基本信息 |
| list_stock_adjusted_quotes | 查询股票复权行情 |
| list_stock_unadjusted_quotes | 查询股票未复权行情 |
| list_stock_income_statements | 查询利润表 |
| list_stock_balance_sheet | 查询资产负债表 |
| list_stock_cash_flows | 查询现金流量表 |
| list_stocks_dividends | 查询股票分红派息 |
| list_stock_rights_issues | 查询配股信息 |
| list_stock_offerings | 查询增发方案 |
| list_stock_major_contracts | 查询重大合同 |
| list_stock_tender_offers | 查询要约收购 |
| list_stock_related_transactions | 查询关联交易 |
| list_stock_earnings_bulletins | 查询业绩快报 |
| list_stock_report_schema | 查询定期报告披露日程 |
| list_stock_pledge_details | 查询股权质押明细 |
| list_stock_freeze_details | 查询股权冻结明细 |
| list_stock_executive_shareholding_change | 查询高管持股变动 |
| list_stock_top10_circulating_shareh | 查询十大流通股东 |
| list_stock_holder_cnt | 查询股东户数 |
| list_stock_institutional_holdings_stats | 查询机构持仓统计 |
| list_stock_management_dirs | 查询管理层信息 |
| list_stock_core_mgmt_changes | 查询核心管理层变更 |
| list_stock_repurchase_plans | 查询股份回购计划 |
| list_stock_capital_changes | 查询股本变动 |
| list_stock_share_adj_factors | 查询除权除息因子 |
| list_stock_industries | 查询股票所属行业 |
| get_stock_basic_info | 查询股票基本信息 |
| get_company_profiles | 查询公司基本信息 |
| get_stock_former_names | 查询股票历史曾用名 |
| get_stock_margin_securities | 查询融资融券标的 |
| list_index_quotes | 查询指数历史行情 |
| list_index_quote_barch | 查询指数日行情 |
| get_index_basic_info | 查询指数基本信息 |
| list_fund_all | 获取全市场基金列表 |
| list_fund_nav_history | 查询基金净值历史 |
| list_fund_adj_navs | 查询基金复权净值 |
| list_fund_adj_quotes | 查询基金前复权行情 |
| list_fund_daily_quotes | 查询基金日行情 |
| list_fund_return_rate | 查询基金历史回报率 |
| list_fund_portfolio_stock_holdings | 查询基金持仓股票 |
| list_fund_portfolio_bond_holdings | 查询基金持仓债券 |
| list_fund_portfolio_asset_holdings | 查询基金资产配置 |
| list_fund_portfolio_fund_holdings | 查询基金持仓基金 |
| list_fund_hold_industry | 查询基金持有行业 |
| list_fund_hold_structures | 查询基金持有人结构 |
| list_etf_constituent_stks | 查询ETF成分股 |
| list_etf_sub_red_lists | 查询ETF申赎清单 |
| list_industry_hold_fund | 查询行业持有基金 |
| get_fund_basic_info | 查询基金基本信息 |
| get_fund_categories | 查询基金三级分类 |
| get_fund_manager_basic_info | 查询基金经理信息 |
| get_fund_listings_record | 查询基金发行上市记录 |
| get_fund_code_assoc | 查询基金关联关系 |
| get_fund_award_records | 查询基金所获奖项 |
| list_fund_invest_targets | 查询基金投资标的 |
| list_fund_perf_benchmarks | 查询基金业绩比较基准 |
| list_fund_fee_structures | 查询基金费率结构 |
| list_fund_fin_inds | 查询基金主要财务指标 |
| list_fund_fin_inds_q | 查询基金季度财务指标 |
| list_fund_share_splits | 查询基金份额拆分折算 |
| list_fund_dividend_distributions | 查询基金分红 |
| list_currency_yield_history | 查询货币基金收益 |
| list_subscription_redemption_status | 查询基金申购赎回状态 |
| list_stock_absorption_mergers | 查询吸收合并事件 |
| list_stock_special_notices | 查询特别提示信息 |
| list_report_institutions | 查询研究机构列表 |
| list_industries | 查询行业列表 |
| get_trade_special_date | 查询交易日衍生日期 |
| is_trade_date | 判断是否为交易日 |
| get_cn_trade_calender_list | 查询A股交易日历 |
| list_economic_cn_cpi | 查询CPI居民消费价格指数 |
| list_economic_cn_ppi | 查询PPI工业生产者出厂价格指数 |
| list_money_supplies | 查询货币供应量M0/M1/M2 |
| list_gover_bond_yield | 查询国债收益率曲线 |
| list_money_market_repo_in | 查询货币市场回购 |
| list_social_financing_sto | 查询社会融资规模存量 |
| list_hk_stock_dividends | 查询港股分红 |
| list_concepts | 查询概念列表 |
| list_concept_hold_fund | 查询概念持有基金 |
| search | 按关键字搜索金融产品 |
| generate_chart | ECharts图表转Base64图片 |
| generate_nex_chart | 生成ECharts图表图片 |

---

### 2. antv-visual（图表可视化）

**功能**: 25种图表生成工具，支持折线图/柱状图/地图等可视化

| 工具名称 | 功能说明 |
|---------|---------|
| generate_line_chart | 生成折线图（展示趋势变化） |
| generate_bar_chart | 生成水平柱状图（分类比较） |
| generate_column_chart | 生成柱状图（分类对比） |
| generate_area_chart | 生成面积图（数据趋势面积） |
| generate_pie_chart | 生成饼图（占比展示） |
| generate_scatter_chart | 生成散点图（两变量关系） |
| generate_radar_chart | 生成雷达图（多维数据） |
| generate_venn_chart | 生成韦恩图（集合关系） |
| generate_mind_map | 生成思维导图（层级结构） |
| generate_organization_chart | 生成组织架构图 |
| generate_flow_diagram | 生成流程图（步骤决策） |
| generate_network_graph | 生成网络图（实体关系） |
| generate_sankey_chart | 生成桑基图（数据流动） |
| generate_funnel_chart | 生成漏斗图（转化率） |
| generate_fishbone_diagram | 生成鱼骨图（因果分析） |
| generate_histogram_chart | 生成直方图（频率分布） |
| generate_boxplot_chart | 生成箱线图（统计摘要） |
| generate_violin_chart | 生成小提琴图（数据分布） |
| generate_treemap_chart | 生成矩形树图（层级数据） |
| generate_word_cloud_chart | 生成词云图（词频权重） |
| generate_liquid_chart | 生成水球图（百分比值） |
| generate_dual_axes_chart | 生成双轴图（趋势+对比） |
| generate_district_map | 生成区域地图（中国行政） |
| generate_path_map | 生成路线地图（旅行规划） |
| generate_pin_map | 生成点标注地图（位置分布） |

---

### 3. amap（高德地图）

**功能**: 高德地图Web服务API，支持地理编码/路径规划/POI搜索

| 工具名称 | 功能说明 |
|---------|---------|
| maps_geo | 地址转经纬度（地理编码） |
| maps_regeocode | 经纬度转行政区划地址 |
| maps_ip_location | IP地址定位 |
| maps_weather | 查询城市天气预报 |
| maps_text_search | 关键词POI搜索 |
| maps_around_search | 周边POI搜索 |
| maps_search_detail | 查询POI详细信息 |
| maps_direction_driving | 驾车路径规划 |
| maps_direction_walking | 步行路径规划 |
| maps_direction_transit_integrated | 公交综合路径规划 |
| maps_bicycling | 骑行路径规划 |
| maps_distance | 距离测量（驾车/步行/球面） |

---

### 4. stock-quote（股票行情）

**功能**: A股/港股/美股/期货/外汇实时行情与K线数据

| 工具名称 | 功能说明 |
|---------|---------|
| A股报价 | A股实时报价 |
| A股排行 | A股涨跌幅/成交量等排行 |
| A股K线 | A股K线数据 |
| A股K线复权 | A股复权K线 |
| 港股报价 | 港股实时报价 |
| 港股排行 | 港股排行 |
| 港股K线 | 港股K线数据 |
| 美股报价 | 美股实时报价 |
| 美股排行 | 美股排行 |
| 美股K线 | 美股K线数据 |
| 美股品种 | 美股品种信息 |
| 外汇报价 | 外汇实时报价 |
| 外汇K线 | 外汇K线数据 |
| 全球指数报价 | 全球指数报价 |
| 全球指数K线 | 全球指数K线 |
| 内盘期货报价 | 内盘期货实时报价 |
| 内盘期货K线 | 内盘期货K线 |
| 内盘期货合约 | 内盘期货合约信息 |
| 外盘期货报价 | 外盘期货实时报价 |
| 外盘期货K线 | 外盘期货K线 |
| 外盘期货合约 | 外盘期货合约信息 |

---

### 5. didi（滴滴出行）

**功能**: 滴滴出行：路径规划/打车/订单管理

| 工具名称 | 功能说明 |
|---------|---------|
| maps_direction_driving | 驾车路径规划 |
| maps_direction_walking | 步行路径规划 |
| maps_direction_transit | 公交地铁路径规划 |
| maps_direction_bicycling | 骑行路径规划 |
| maps_textsearch | 地点关键词搜索 |
| maps_place_around | 周边地点搜索 |
| maps_regeocode | 经纬度转地址 |
| taxi_estimate | 查看打车预估价格 |
| taxi_create_order | 创建打车订单 |
| taxi_cancel_order | 取消打车订单 |
| taxi_query_order | 查询订单状态 |
| taxi_get_driver_location | 获取司机实时位置 |
| taxi_generate_ride_app_link | 生成打车App深度链接 |

---

### 6. github（GitHub操作）

**功能**: GitHub仓库/Issue/PR/代码管理

| 工具名称 | 功能说明 |
|---------|---------|
| create_repository | 创建新仓库 |
| fork_repository | Fork仓库 |
| get_file_contents | 获取文件/目录内容 |
| push_files | 批量推送文件 |
| create_or_update_file | 创建或更新单文件 |
| create_branch | 创建分支 |
| list_commits | 获取提交记录 |
| search_repositories | 搜索仓库 |
| search_code | 搜索代码 |
| search_users | 搜索用户 |
| create_issue | 创建Issue |
| list_issues | 列出Issue |
| get_issue | 获取Issue详情 |
| update_issue | 更新Issue |
| add_issue_comment | 添加Issue评论 |
| search_issues | 搜索Issue/PR |
| create_pull_request | 创建PR |
| list_pull_requests | 列出PR |
| get_pull_request | 获取PR详情 |
| get_pull_request_files | 获取PR变更文件 |
| get_pull_request_comments | 获取PR评论 |
| get_pull_request_reviews | 获取PR审查 |
| get_pull_request_status | 获取PR状态 |
| create_pull_request_review | 创建PR审查 |
| merge_pull_request | 合并PR |
| update_pull_request_branch | 更新PR分支 |

---

### 7. minimax（MiniMax AI）

**功能**: MiniMax AI：图片/视频/音乐生成，语音合成与克隆

| 工具名称 | 功能说明 |
|---------|---------|
| text_to_image | 文字生成图片 |
| text_to_audio | 文字转语音 |
| text_to_video | 文字生成视频 |
| music_generation | AI音乐生成 |
| voice_clone | 声音克隆 |
| voice_design | AI生成语音 |
| list_voices | 列出可用音色 |
| play_audio | 播放音频文件 |
| query_video_generation | 查询视频生成状态 |

---

### 8. weather（天气查询）

**功能**: 实时天气/预报/空气质量

| 工具名称 | 功能说明 |
|---------|---------|
| get_weather | 获取当前天气 |
| get_forecast | 获取天气预报（1-5天） |
| get_air_quality | 获取空气质量 |

---

### 9. local_time（本地时间）

**功能**: 获取当前本地时间

| 工具名称 | 功能说明 |
|---------|---------|
| get_current_time | 获取当前本地时间 |

---

### 10. bmi-mcp（BMI指数）

**功能**: BMI体重指数计算与健康评估

| 工具名称 | 功能说明 |
|---------|---------|
| BMI体重指数 | 根据身高体重计算BMI，返回健康评估与建议 |

---

### 11. bw-ir（发票验证）

**功能**: 增值税发票/普通发票真实性核验

| 工具名称 | 功能说明 |
|---------|---------|
| invoice_verification | 验证发票真伪与合规性，支持14类票据 |

---

### 12. food-detective（美食推荐）

**功能**: 地方美食推荐

| 工具名称 | 功能说明 |
|---------|---------|
| 推荐美食 | 传入地名，返回5条当地美食和推荐理由 |

---

### 13. how-to-cook（菜谱查询）

**功能**: 菜谱查询与膳食推荐

| 工具名称 | 功能说明 |
|---------|---------|
| mcp_howtocook_getAllRecipes | 获取所有菜谱 |
| mcp_howtocook_getRecipesByCategory | 按分类查询菜谱（水产/早餐/荤菜/素菜等） |
| mcp_howtocook_getRecipeById | 按名称/ID查询菜谱详情（食材+步骤） |
| mcp_howtocook_whatToEat | 根据人数推荐菜品组合 |
| mcp_howtocook_recommendMeals | 智能推荐一周膳食计划，含购物清单 |

---

### 14. market-cmapi（地区新闻）

**功能**: 中国各省市地区新闻查询

| 工具名称 | 功能说明 |
|---------|---------|
| 查询地区新闻 | 按地区ID/名称查询新闻 |
| 查询支持的新闻地区 | 查询API支持的省市列表 |

---

### 15. openscad（3D建模）

**功能**: AI 3D建模与图片生成

| 工具名称 | 功能说明 |
|---------|---------|
| create_3d_model | 自然语言生成3D模型 |
| modify_3d_model | 修改现有3D模型 |
| export_model | 导出3D模型（STL等格式） |
| list_models | 列出所有生成的模型 |
| get_supported_3d_shapes | 获取支持的3D形状类型 |
| generate_image | Venice.ai图片生成 |
| generate_image_gemini | Google Gemini图片生成 |

---

### 16. vision-mcp（图片分析）

**功能**: AI图片内容分析与OCR识别

| 工具名称 | 功能说明 |
|---------|---------|
| analyze_image | 分析图片内容并提供详细描述 |

---

### 17. gezhe（PPT生成）

**功能**: AI自动生成PPT演示文稿

| 工具名称 | 功能说明 |
|---------|---------|
| generate_ppt_by_topic | 输入主题，自动生成PPT |

---

### 18. playwright（浏览器自动化）

**功能**: 浏览器自动化操作与网页抓取

| 工具名称 | 功能说明 |
|---------|---------|
| navigate | 导航到指定URL |
| screenshot | 页面截图 |
| get_page_content | 获取页面HTML内容 |
| get_text | 获取元素文本内容 |
| click | 点击页面元素 |
| fill | 填写表单字段 |
| wait_for_selector | 等待元素出现 |
| close_browser | 关闭浏览器 |

---

### 19. pandoc（文档转换）

**功能**: 文档格式转换（Markdown/HTML/PDF/DOCX等）

| 工具名称 | 功能说明 |
|---------|---------|
| convert-contents | 内容格式转换（支持PDF/DOCX/HTML等） |

---

### 20. doc-forge（文档处理）

**功能**: PDF/DOCX/HTML/Excel等文档处理工具

| 工具名称 | 功能说明 |
|---------|---------|
| document_reader | 读取PDF/DOCX/TXT等文档 |
| pdf_merger | 合并多个PDF |
| pdf_splitter | 拆分PDF |
| docx_to_pdf | DOCX转PDF |
| docx_to_html | DOCX转HTML |
| html_to_markdown | HTML转Markdown |
| html_to_text | HTML转纯文本 |
| html_cleaner | 清理HTML冗余标签 |
| html_formatter | 格式化HTML代码 |
| html_extract_resources | 提取HTML资源（图片/视频/链接） |
| text_diff | 比较两个文本文件差异 |
| text_splitter | 按分隔符/行数拆分文本 |
| text_formatter | 格式化文本（缩进/行距） |
| text_encoding_converter | 文本编码转换 |
| excel_read | 读取Excel并转为JSON |
| format_convert | 文档格式互转（Markdown/HTML/XML/JSON） |

---

### 21. excel（Excel操作）

**功能**: Excel读取/写入/格式化

| 工具名称 | 功能说明 |
|---------|---------|
| excel_read_sheet | 读取Excel工作表（支持分页） |
| excel_write_to_sheet | 写入数据到工作表 |
| excel_format_range | 格式化单元格区域 |
| excel_create_table | 创建Excel表格 |
| excel_copy_sheet | 复制工作表 |
| excel_describe_sheets | 列出所有工作表信息 |

---

### 22. qrcode-mcp（二维码）

**功能**: 二维码生成

| 工具名称 | 功能说明 |
|---------|---------|
| 二维码生成 | 将文本/URL生成为二维码图片 |

---

### 23. sqlite（数据库）

**功能**: SQLite数据库操作

| 工具名称 | 功能说明 |
|---------|---------|
| list_tables | 列出所有表 |
| describe_table | 获取表结构 |
| read_query | 执行SELECT查询 |
| write_query | 执行INSERT/UPDATE/DELETE |
| create_table | 创建新表 |

---

## 未连接/已禁用MCP

| MCP名称 | 状态 | 说明 |
|--------|------|------|
| luckin | ✗ disabled | 瑞幸咖啡MCP（已禁用） |
| mbti | ✗ disabled | MBTI性格测试MCP（已禁用） |
| mmb-mcp | ✗ 401错误 | 慢慢买MCP（认证失败） |
| gf-windmill | ✗ disabled | 券商MCP（已禁用） |
| xhs-toolkit | ✗ 超时 | 小红书MCP（连接超时） |
| xhs-toolkit-http | ✗ 连接失败 | 小红书HTTP服务（未启动） |

---

*📌 文档由 Hermes Agent 自动生成*
