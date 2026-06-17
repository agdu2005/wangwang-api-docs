# Hermes Agent MCP API 文档

> 📅 更新时间: 2026-06-17  
> 🤖 Hermes Agent 版本: 最新  
> 📊 总计: 28个已启用MCP服务器

---

## 📋 目录

1. [HTTP传输型MCP](#http传输型mcp)
2. [SSE传输型MCP](#sse传输型mcp)
3. [Stdio传输型MCP](#stdio传输型mcp)

---

## HTTP传输型MCP

### 1. antv-chart (金融数据)

**功能**: A股/基金/指数的金融数据查询与分析

| 工具名称 | 功能说明 |
|---------|---------|
| list_fund_nav_history | 查询基金历史净值 |
| list_fund_adj_navs | 查询基金复权净值 |
| list_fund_adj_quotes | 查询基金前复权日行情 |
| list_fund_daily_quotes | 查询基金日行情 |
| list_fund_return_rate | 查询基金回报率 |
| list_fund_portfolio_stock_holdings | 查询基金持仓股票 |
| list_fund_portfolio_bond_holdings | 查询基金持仓债券 |
| list_fund_portfolio_asset_holdings | 查询基金资产配置 |
| list_fund_hold_industry | 查询基金持有行业 |
| list_fund_hold_structures | 查询基金持有人结构 |
| list_etf_constituent_stks | 查询ETF成分股 |
| list_etf_sub_red_lists | 查询ETF申赎清单 |
| list_index_quotes | 查询指数行情 |
| list_index_quote_barch | 查询指数历史行情 |
| list_stock_all | 查询全市场股票 |
| list_stock_adjusted_quotes | 查询股票复权行情 |
| list_stock_unadjusted_quotes | 查询股票未复权行情 |
| list_stock_income_statements | 查询利润表 |
| list_stock_balance_sheet | 查询资产负债表 |
| list_stock_cash_flows | 查询现金流量表 |
| list_stock_cash_flows_pit | 查询现金流时点数据 |
| list_stocks_dividends | 查询股票分红 |
| list_stock_rights_issues | 查询配股 |
| list_stock_offerings | 查询增发 |
| list_stock_major_contracts | 查询重大合同 |
| list_stock_tender_offers | 查询要约收购 |
| list_stock_related_transactions | 查询关联交易 |
| list_stock_earnings_bulletins | 查询业绩快报 |
| list_stock_report_schema | 查询定期报告 |
| list_stock_pledge_details | 查询股权质押 |
| list_stock_freeze_details | 查询股权冻结 |
| list_stock_executive_shareholding_change | 查询高管持股变动 |
| list_stock_top10_circulating_shareh | 查询十大流通股东 |
| list_stock_holder_cnt | 查询股东户数 |
| list_stock_institutional_holdings_stats | 查询机构持仓统计 |
| list_stock_management_dirs | 查询管理层信息 |
| list_stock_core_mgmt_changes | 查询核心管理层变更 |
| list_stock_repurchase_plans | 查询股份回购 |
| list_stock_capital_changes | 查询股本变动 |
| list_stock_share_adj_factors | 查询除权除息因子 |
| list_stock_industries | 查询股票行业 |
| list_stock_industries | 查询股票行业分类 |
| get_company_profiles | 查询公司基本信息 |
| get_fund_basic_info | 查询基金基本信息 |
| get_fund_categories | 查询基金分类 |
| get_fund_manager_basic_info | 查询基金经理 |
| get_fund_listings_record | 查询基金发行上市 |
| get_fund_fee_structures | 查询基金费率 |
| get_fund_perf_benchmarks | 查询基金业绩基准 |
| get_fund_invest_targets | 查询基金投资标的 |
| list_fund_all | 查询全部基金 |
| list_fund_fin_inds | 查询基金财务指标 |
| list_fund_fin_inds_q | 查询基金季度财务指标 |
| list_fund_dividend_distributions | 查询基金分红 |
| list_fund_share_splits | 查询基金拆分折算 |
| list_fund_shares | 查询基金份额变动 |
| list_subscription_redemption_status | 查询申赎状态 |
| get_index_basic_info | 查询指数基本信息 |
| list_industries | 查询行业列表 |
| list_industry_hold_fund | 查询行业持有基金 |
| list_concepts | 查询概念列表 |
| list_concept_hold_fund | 查询概念持有基金 |
| list_stock_special_notices | 查询特别提示 |
| list_stock_absorption_mergers | 查询吸收合并 |
| list_stock_stock_plans | 查询股票计划 |
| list_stock_management_plans | 查询管理层计划 |
| list_stock_related_parties | 查询关联方 |
| list_stock_management_changes | 查询管理层变动 |
| list_stock_related_party_transactions | 查询关联方交易 |
| list_stock_management_compensation | 查询管理层薪酬 |
| search | 搜索金融产品 |
| list_gover_bond_yield | 查询国债收益率 |
| list_money_market_repo_in | 查询货币市场 |
| list_money_supplies | 查询货币供应量 |
| list_social_financing_sto | 查询社融存量 |
| list_economic_cn_cpi | 查询CPI |
| list_economic_cn_ppi | 查询PPI |
| list_trade_special_date | 查询交易日衍生日期 |
| is_trade_date | 判断是否交易日 |
| get_trade_calender_list | 查询交易日历 |
| get_stock_basic_info | 查询股票基本信息 |
| get_stock_industries | 查询股票行业 |
| get_stock_margin_securities | 查询融资融券标的 |
| get_stock_rights_issues | 查询配股 |
| get_stock_former_names | 查询股票曾用名 |
| list_stock_management_plans | 查询管理层计划 |
| list_stock_management_changes | 查询管理层变更 |
| list_stock_related_party_transactions | 查询关联方交易 |
| list_stock_management_compensation | 查询管理层薪酬 |
| list_hk_stock_dividends | 查询港股分红 |
| list_stock_mgmt_reports | 查询管理报告 |
| list_stock_audit_reports | 查询审计报告 |
| list_stock_prospectus | 查询招股说明书 |
| list_stock_ipo_info | 查询IPO信息 |
| list_stock_split_info | 查询拆分信息 |
| list_stock_delist_info | 查询退市信息 |
| generate_chart | 生成图表 |

---

### 2. stock-quote (股票行情)

**功能**: A股K线、外汇、期货行情查询

| 工具名称 | 功能说明 |
|---------|---------|
| A_K_ | A股K线行情 |
| A_K___ | A股K线复权 |
| A___ | A股排行 |
| ___K_ | 外汇K线 |
| _____ | 外汇报价 |
| _____K_ | 外盘期货K线 |
| _______ | 外盘期货报价 |

---

### 3. didi (滴滴出行)

**功能**: 滴滴打车、路线规划、地点搜索

| 工具名称 | 功能说明 |
|---------|---------|
| maps_direction_driving | 驾车路径规划 |
| maps_direction_bicycling | 骑行路径规划 |
| maps_direction_walking | 步行路径规划 |
| maps_direction_transit | 公交路径规划 |
| maps_textsearch | 地点关键词搜索 |
| maps_place_around | 周边地点搜索 |
| maps_regeocode | 经纬度转地址 |
| taxi_estimate | 打车预估价格 |
| taxi_create_order | 创建打车订单 |
| taxi_query_order | 查询订单状态 |
| taxi_cancel_order | 取消订单 |
| taxi_get_driver_location | 获取司机位置 |
| taxi_generate_ride_app_link | 生成打车链接 |

---

### 4. bmi-mcp (BMI指数)

**功能**: BMI体重指数计算与健康评估

| 工具名称 | 功能说明 |
|---------|---------|
| BMI____ | 计算BMI及健康建议 |

---

### 5. qrcode-mcp (二维码)

**功能**: 生成二维码图片

| 工具名称 | 功能说明 |
|---------|---------|
| ______ | 生成二维码 |

---

### 6. gezhe (PPT生成)

**功能**: AI生成PPT演示文稿

| 工具名称 | 功能说明 |
|---------|---------|
| generate_ppt_by_topic | 根据主题生成PPT |

---

### 7. bmi-mcp (健康指数)

**功能**: 身体健康指数计算

| 工具名称 | 功能说明 |
|---------|---------|
| BMI____ | BMI计算与健康建议 |

---

### 8. bw-ir (发票验证)

**功能**: 增值税发票真伪查验

| 工具名称 | 功能说明 |
|---------|---------|
| invoice_verification | 发票验证 |

---

### 9. food-detective (美食推荐)

**功能**: 各地美食推荐

| 工具名称 | 功能说明 |
|---------|---------|
| ______ | 查询地方美食推荐 |

---

### 10. market-cmapi (区域新闻)

**功能**: 各省市区域新闻查询

| 工具名称 | 功能说明 |
|---------|---------|
| _______ | 查询区域新闻 |
| __________ | 查询支持区域 |

---

### 11. how-to-cook (菜谱)

**功能**: 中华菜谱大全

| 工具名称 | 功能说明 |
|---------|---------|
| getAllRecipes | 获取所有菜谱 |
| getRecipeById | 按ID查询菜谱 |
| getRecipesByCategory | 按分类查询菜谱 |
| whatToEat | 随机推荐菜品 |
| recommendMeals | 智能推荐膳食 |

---

### 12. minimax (AI内容生成)

**功能**: 文本/图片/视频/音乐/语音生成

| 工具名称 | 功能说明 |
|---------|---------|
| text_to_image | 文本生成图片 |
| generate_video | 文本/图片生成视频 |
| music_generation | AI音乐生成 |
| text_to_audio | 文本转语音 |
| voice_clone | 语音克隆 |
| voice_design | 语音设计 |
| list_voices | 列出可用音色 |
| play_audio | 播放音频 |
| query_video_generation | 查询视频生成状态 |

---

### 13. antv-visual (可视化图表)

**功能**: 多种图表可视化生成

| 工具名称 | 功能说明 |
|---------|---------|
| generate_bar_chart | 生成柱状图 |
| generate_column_chart | 生成条形图 |
| generate_line_chart | 生成折线图 |
| generate_area_chart | 生成面积图 |
| generate_pie_chart | 生成饼图 |
| generate_scatter_chart | 生成散点图 |
| generate_funnel_chart | 生成漏斗图 |
| generate_radar_chart | 生成雷达图 |
| generate_mind_map | 生成思维导图 |
| generate_flow_diagram | 生成流程图 |
| generate_organization_chart | 生成组织图 |
| generate_network_graph | 生成网络图 |
| generate_fishbone_diagram | 生成鱼骨图 |
| generate_sankey_chart | 生成桑基图 |
| generate_treemap_chart | 生成矩形树图 |
| generate_boxplot_chart | 生成箱线图 |
| generate_violin_chart | 生成小提琴图 |
| generate_histogram_chart | 生成直方图 |
| generate_word_cloud_chart | 生成词云图 |
| generate_liquid_chart | 生成水球图 |
| generate_venn_chart | 生成韦恩图 |
| generate_district_map | 生成区域地图 |
| generate_path_map | 生成路线地图 |
| generate_pin_map | 生成标点地图 |
| generate_dual_axes_chart | 生成双轴图表 |

---

### 14. mmb-mcp (音乐生成)

**功能**: Suno风格音乐生成

| 工具名称 | 功能说明 |
|---------|---------|
| music_generation | AI音乐生成 |

---

## SSE传输型MCP

### 15. amap (高德地图)

**功能**: 高德地图服务

| 工具名称 | 功能说明 |
|---------|---------|
| maps_geo | 地址转经纬度 |
| maps_regeocode | 经纬度转地址 |
| maps_direction_driving | 驾车导航 |
| maps_direction_walking | 步行导航 |
| maps_direction_bicycling | 骑行导航 |
| maps_direction_transit_integrated | 公交导航 |
| maps_text_search | 关键词搜索 |
| maps_around_search | 周边搜索 |
| maps_search_detail | 搜索详情 |
| maps_distance | 距离测量 |
| maps_ip_location | IP定位 |
| maps_weather | 天气预报 |

---

### 16. weather (天气预报)

**功能**: 天气查询

| 工具名称 | 功能说明 |
|---------|---------|
| get_weather | 获取当前天气 |
| get_forecast | 获取天气预报 |
| get_air_quality | 获取空气质量 |

---

### 17. local_time (本地时间)

**功能**: 获取本地时间

| 工具名称 | 功能说明 |
|---------|---------|
| get_current_time | 获取当前时间 |

---

### 18. vision-mcp (视觉理解)

**功能**: 图片/视频理解与分析

| 工具名称 | 功能说明 |
|---------|---------|
| analyze_image | 分析图片内容 |

---

## Stdio传输型MCP

### 19. github (GitHub操作)

**功能**: GitHub仓库/PR/Issue管理

| 工具名称 | 功能说明 |
|---------|---------|
| get_file_contents | 获取文件内容 |
| push_files | 推送多个文件 |
| create_repository | 创建仓库 |
| fork_repository | Fork仓库 |
| create_branch | 创建分支 |
| create_pull_request | 创建PR |
| merge_pull_request | 合并PR |
| get_pull_request | 获取PR详情 |
| list_pull_requests | 列出PR |
| get_pull_request_files | 获取PR文件 |
| get_pull_request_reviews | 获取PR审查 |
| get_pull_request_comments | 获取PR评论 |
| create_pull_request_review | 创建PR审查 |
| list_commits | 列出提交 |
| get_issue | 获取Issue |
| list_issues | 列出Issue |
| create_issue | 创建Issue |
| update_issue | 更新Issue |
| add_issue_comment | 添加Issue评论 |
| search_repositories | 搜索仓库 |
| search_issues | 搜索Issue |
| search_code | 搜索代码 |
| search_users | 搜索用户 |
| update_pull_request_branch | 更新PR分支 |
| get_pull_request_status | 获取PR状态 |

---

### 20. sqlite (SQLite数据库)

**功能**: 本地SQLite数据库操作

| 工具名称 | 功能说明 |
|---------|---------|
| list_tables | 列出表 |
| describe_table | 表结构 |
| read_query | 读取查询 |
| write_query | 写入/更新/删除 |
| create_table | 创建表 |

---

### 21. playwright (浏览器自动化)

**功能**: 浏览器自动化操作

| 工具名称 | 功能说明 |
|---------|---------|
| navigate | 导航到URL |
| screenshot | 截图 |
| click | 点击元素 |
| fill | 填写表单 |
| get_text | 获取文本 |
| get_page_content | 获取页面内容 |
| wait_for_selector | 等待元素 |
| close_browser | 关闭浏览器 |

---

### 22. pandoc (文档转换)

**功能**: 文档格式转换

| 工具名称 | 功能说明 |
|---------|---------|
| convert_contents | 转换内容格式 |

---

### 23. doc-forge (文档处理)

**功能**: PDF/Word/Excel处理

| 工具名称 | 功能说明 |
|---------|---------|
| excel_read | 读取Excel |
| excel_write_to_sheet | 写入Excel |
| excel_format_range | 格式化单元格 |
| excel_create_table | 创建表格 |
| excel_describe_sheets | 列出工作表 |
| excel_copy_sheet | 复制工作表 |
| pdf_merger | 合并PDF |
| pdf_splitter | 拆分PDF |
| document_reader | 读取文档 |
| docx_to_html | DOCX转HTML |
| docx_to_pdf | DOCX转PDF |
| html_to_markdown | HTML转Markdown |
| html_to_text | HTML转文本 |
| html_cleaner | 清理HTML |
| html_formatter | 格式化HTML |
| html_extract_resources | 提取资源 |
| format_convert | 格式转换 |
| text_encoding_converter | 编码转换 |
| text_formatter | 文本格式化 |
| text_diff | 文本对比 |
| text_splitter | 文本分割 |

---

### 24. excel (Excel处理)

**功能**: Excel操作

| 工具名称 | 功能说明 |
|---------|---------|
| excel_read | 读取Excel |
| excel_write_to_sheet | 写入Excel |
| excel_format_range | 格式化 |
| excel_create_table | 创建表格 |
| excel_describe_sheets | 列出工作表 |
| excel_copy_sheet | 复制工作表 |

---

### 25. openscad (3D建模)

**功能**: 3D模型生成与导出

| 工具名称 | 功能说明 |
|---------|---------|
| create_3d_model | 创建3D模型 |
| modify_3d_model | 修改3D模型 |
| export_model | 导出模型 |
| list_models | 列出模型 |
| generate_image | 生成图片 |
| generate_image_gemini | Gemini生成图片 |
| get_supported_3d_shapes | 支持的形状 |

---

### 26. xhs-toolkit (小红书)

**功能**: 小红书内容工具

| 工具名称 | 功能说明 |
|---------|---------|
| search_notes | 搜索笔记 |
| get_note_detail | 获取笔记详情 |
| get_home_feed | 获取首页推荐 |

---

### 27. xhs-toolkit-http (小红书HTTP)

**功能**: 小红书HTTP API

| 工具名称 | 功能说明 |
|---------|---------|
| (HTTP API接口) | 小红书API调用 |

---

### 28. qrcode-mcp (二维码生成)

**功能**: 本地二维码生成与识别

| 工具名称 | 功能说明 |
|---------|---------|
| qrcode_generator | 生成二维码 |

---

## 统计汇总

| 传输类型 | 已启用数量 |
|---------|----------|
| HTTP | 11 |
| SSE | 6 |
| Stdio | 11 |
| **总计** | **28** |

---

*文档由Hermes Agent自动生成*
