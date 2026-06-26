# Hermes Agent MCP API 文档

> 🤖 Powered by Hermes Agent | 更新日期：2026年06月26日 08:02 CST

**⚠️ 状态说明** | 🟢 enabled = 已启用 | 🔴 disabled = 已禁用 | ❌ failed = 连接失败

---

## MCP 服务总览（24个已启用 / 2个已禁用 / 3个失败）

| 状态 | 数量 | MCP名称 |
|------|------|---------|
| 🟢 enabled | 24 | antv-chart, antv-visual, bmi-mcp, bw-ir, didi, food-detective, how-to-cook, market-cmapi, openscad, vision-mcp, gezhe, playwright, pandoc, doc-forge, excel, minimax, qrcode-mcp, stock-quote, amap, github, sqlite, weather, local_time, xhs-toolkit |
| 🔴 disabled | 2 | luckin, mbti |
| ❌ failed | 3 | mmb-mcp (401认证失败), xhs-toolkit-http (本地服务未启动) |

---

## 1. antv-chart — A股/基金/指数金融数据

**工具数量**: 100+ | **状态**: 🟢 enabled

功能全面的A股/基金/指数/债券/宏观经济数据查询接口。

### 股票数据

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_chart_list_stock_all` | 获取全市场A股/B股股票基本信息列表 |
| `mcp_antv_chart_get_stock_basic_info` | 查询股票基本信息（名称、板块、上市状态等） |
| `mcp_antv_chart_get_company_profiles` | 查询公司基本信息（注册、资本等） |
| `mcp_antv_chart_list_stock_industries` | 查询股票所属申万行业分类 |
| `mcp_antv_chart_list_stock_balance_sheet` | 查询股票资产负债表 |
| `mcp_antv_chart_list_stock_income_statements` | 查询股票利润表 |
| `mcp_antv_chart_list_stock_cash_flows` | 查询股票现金流量表 |
| `mcp_antv_chart_list_stock_adjusted_quotes` | 查询股票复权行情 |
| `mcp_antv_chart_list_stock_unadjusted_quotes` | 查询股票未复权行情 |
| `mcp_antv_chart_list_stocks_dividends` | 查询股票分红派息 |
| `mcp_antv_chart_list_stock_share_adj_factors` | 查询除权除息事件 |
| `mcp_antv_chart_list_stock_capital_changes` | 查询公司股本变动历史 |
| `mcp_antv_chart_list_stock_holder_cnt` | 查询股东户数及持股结构 |
| `mcp_antv_chart_list_stock_top10_circulating_shareh` | 查询前十大流通股东 |
| `mcp_antv_chart_list_stock_management_dirs` | 查询管理层人员信息 |
| `mcp_antv_chart_list_stock_core_mgmt_changes` | 查询核心管理层变更记录 |
| `mcp_antv_chart_list_stock_institutional_holdings_stats` | 查询机构持股统计 |
| `mcp_antv_chart_list_stock_executive_shareholding_change` | 查询高管持股变动 |
| `mcp_antv_chart_list_stock_pledge_details` | 查询股权质押明细 |
| `mcp_antv_chart_list_stock_freeze_details` | 查询股权冻结明细 |
| `mcp_antv_chart_list_stock_offerings` | 查询增发方案详情 |
| `mcp_antv_chart_list_stocks_public_offering_place` | 查询公开增发/配售结果 |
| `mcp_antv_chart_list_stocks_rights_issue_res` | 查询配股发行结果 |
| `mcp_antv_chart_list_stock_tender_offers` | 查询要约收购事件 |
| `mcp_antv_chart_list_stock_repurchase_plans` | 查询股份回购计划 |
| `mcp_antv_chart_list_stock_absorption_mergers` | 查询吸收合并事件 |
| `mcp_antv_chart_list_stock_related_transactions` | 查询关联交易明细 |
| `mcp_antv_chart_list_stock_major_contracts` | 查询重大合同公告 |
| `mcp_antv_chart_list_stock_report_schema` | 查询定期报告预披露日程 |
| `mcp_antv_chart_list_stock_special_notices` | 查询股票特别提示 |
| `mcp_antv_chart_list_stock_earnings_bulletins` | 查询业绩快报 |
| `mcp_antv_chart_list_stock_margin_securities` | 查询融资融券标的 |
| `mcp_antv_chart_get_stock_rights_issues` | 查询配股发行信息 |
| `mcp_antv_chart_list_stock_former_names` | 查询股票历史曾用名 |
| `mcp_antv_chart_get_stock_industries` | 查询股票行业分类 |

### 基金数据

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_chart_list_fund_all` | 获取全市场基金列表 |
| `mcp_antv_chart_get_fund_basic_info` | 查询基金基本信息 |
| `mcp_antv_chart_get_fund_categories` | 查询基金三级分类 |
| `mcp_antv_chart_get_fund_manager_basic_info` | 查询基金经理信息 |
| `mcp_antv_chart_list_fund_nav_history` | 查询基金历史净值 |
| `mcp_antv_chart_list_fund_adj_navs` | 查询基金复权净值 |
| `mcp_antv_chart_list_fund_adj_quotes` | 查询基金前复权行情 |
| `mcp_antv_chart_list_fund_daily_quotes` | 查询基金日行情 |
| `mcp_antv_chart_list_fund_return_rate` | 查询基金历史回报率 |
| `mcp_antv_chart_list_fund_portfolio_stock_holdings` | 查询基金持仓股票 |
| `mcp_antv_chart_list_fund_portfolio_bond_holdings` | 查询基金持仓债券 |
| `mcp_antv_chart_list_fund_portfolio_asset_holdings` | 查询基金资产配置 |
| `mcp_antv_chart_list_portfolio_fund_holdings` | 查询基金持仓基金 |
| `mcp_antv_chart_list_fund_hold_structures` | 查询基金持有人结构 |
| `mcp_antv_chart_list_fund_hold_industry` | 查询基金行业配置 |
| `mcp_antv_chart_list_etf_constituent_stks` | 查询ETF成分股 |
| `mcp_antv_chart_list_etf_sub_red_lists` | 查询ETF申购赎回清单 |
| `mcp_antv_chart_list_fund_fee_structures` | 查询基金费率结构 |
| `mcp_antv_chart_list_fund_perf_benchmarks` | 查询基金业绩基准 |
| `mcp_antv_chart_list_fund_invest_targets` | 查询基金投资标的 |
| `mcp_antv_chart_list_fund_dividend_distributions` | 查询基金分红信息 |
| `mcp_antv_chart_list_fund_share_splits` | 查询基金拆分折算 |
| `mcp_antv_chart_list_fund_shares` | 查询基金份额变动 |
| `mcp_antv_chart_list_subscription_redemption_status` | 查询基金申赎状态 |
| `mcp_antv_chart_list_fund_fin_inds` | 查询基金财务指标 |
| `mcp_antv_chart_list_fund_fin_inds_q` | 查询基金季度财务指标 |
| `mcp_antv_chart_list_currency_yield_history` | 查询货币基金收益 |
| `mcp_antv_chart_get_fund_code_assoc` | 查询基金关联关系 |
| `mcp_antv_chart_get_fund_award_records` | 查询基金所获奖项 |
| `mcp_antv_chart_list_fund_listings_record` | 查询基金发行上市信息 |

### 指数数据

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_chart_get_index_basic_info` | 查询指数基本信息 |
| `mcp_antv_chart_list_index_quotes` | 查询指数历史行情 |
| `mcp_antv_chart_list_index_quote_barch` | 查询指数条形行情 |
| `mcp_antv_chart_list_perf_benchmark_quote` | 查询基准指数行情 |

### 宏观/其他

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_chart_search` | 金融产品关键字搜索 |
| `mcp_antv_chart_list_industries` | 行业列表查询 |
| `mcp_antv_chart_list_concepts` | 概念板块列表 |
| `mcp_antv_chart_list_concept_hold_fund` | 概念持仓基金 |
| `mcp_antv_chart_list_industry_hold_fund` | 行业持仓基金 |
| `mcp_antv_chart_get_cn_trade_calender_list` | A股交易日历 |
| `mcp_antv_chart_get_trade_special_date` | 交易日衍生日期 |
| `mcp_antv_chart_is_trade_date` | 判断是否交易日 |
| `mcp_antv_chart_generate_chart` | ECharts图表生成图片 |
| `mcp_antv_chart_generate_nex_chart` | ECharts图表生成（Nex版） |
| `mcp_antv_chart_list_hk_stock_dividends` | 港股分红派息 |
| `mcp_antv_chart_list_economic_cn_cpi` | 中国CPI数据 |
| `mcp_antv_chart_list_economic_cn_ppi` | 中国PPI数据 |
| `mcp_antv_chart_list_money_supplies` | 货币供应量数据 |
| `mcp_antv_chart_list_gover_bond_yield` | 国债收益率曲线 |
| `mcp_antv_chart_list_money_market_repo_in` | 货币市场数据 |
| `mcp_antv_chart_list_social_financing_sto` | 社会融资规模存量 |
| `mcp_antv_chart_list_report_institutions` | 研究机构列表 |

---

## 2. antv-visual — 可视化图表生成

**工具数量**: 25 | **状态**: 🟢 enabled

生成各类可视化图表，支持面积图、柱状图、饼图、地图、词云等。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_visual_generate_area_chart` | 生成面积图，展示数据趋势 |
| `mcp_antv_visual_generate_bar_chart` | 生成水平条形图 |
| `mcp_antv_visual_generate_column_chart` | 生成柱状图 |
| `mcp_antv_visual_generate_boxplot_chart` | 生成箱线图 |
| `mcp_antv_visual_generate_pie_chart` | 生成饼图/环形图 |
| `mcp_antv_visual_generate_line_chart` | 生成折线图 |
| `mcp_antv_visual_generate_scatter_chart` | 生成散点图 |
| `mcp_antv_visual_generate_radar_chart` | 生成雷达图 |
| `mcp_antv_visual_generate_funnel_chart` | 生成漏斗图 |
| `mcp_antv_visual_generate_histogram_chart` | 生成直方图 |
| `mcp_antv_visual_generate_sankey_chart` | 生成桑基图 |
| `mcp_antv_visual_generate_treemap_chart` | 生成矩形树图 |
| `mcp_antv_visual_generate_venn_chart` | 生成韦恩图 |
| `mcp_antv_visual_generate_violin_chart` | 生成小提琴图 |
| `mcp_antv_visual_generate_word_cloud_chart` | 生成词云图 |
| `mcp_antv_visual_generate_mind_map` | 生成思维导图 |
| `mcp_antv_visual_generate_organization_chart` | 生成组织架构图 |
| `mcp_antv_visual_generate_flow_diagram` | 生成流程图 |
| `mcp_antv_visual_generate_fishbone_diagram` | 生成鱼骨图 |
| `mcp_antv_visual_generate_network_graph` | 生成关系网络图 |
| `mcp_antv_visual_generate_dual_axes_chart` | 生成双轴图（柱+线） |
| `mcp_antv_visual_generate_district_map` | 生成区域地图 |
| `mcp_antv_visual_generate_pin_map` | 生成点标注地图 |
| `mcp_antv_visual_generate_path_map` | 生成路线规划地图 |
| `mcp_antv_visual_generate_liquid_chart` | 生成水球图 |

---

## 3. didi — 滴滴出行

**工具数量**: 13 | **状态**: 🟢 enabled

网约车出行服务，包含预估、下单、查询、路线规划。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_didi_taxi_estimate` | 查询网约车预估价格 |
| `mcp_didi_taxi_create_order` | 创建打车订单 |
| `mcp_didi_taxi_query_order` | 查询订单状态 |
| `mcp_didi_taxi_cancel_order` | 取消打车订单 |
| `mcp_didi_taxi_get_driver_location` | 获取司机实时位置 |
| `mcp_didi_taxi_generate_ride_app_link` | 生成打车深度链接 |
| `mcp_didi_maps_direction_driving` | 驾车路径规划 |
| `mcp_didi_maps_direction_transit` | 公交路线规划 |
| `mcp_didi_maps_direction_bicycling` | 骑行路线规划 |
| `mcp_didi_maps_direction_walking` | 步行路线规划 |
| `mcp_didi_maps_place_around` | 周边地点搜索 |
| `mcp_didi_maps_textsearch` | 关键词地点搜索 |
| `mcp_didi_maps_regeocode` | 经纬度转地址 |

---

## 4. amap — 高德地图

**工具数量**: 12 | **状态**: 🟢 enabled

高德地图服务，包含地理编码、路径规划、天气、POI搜索。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_amap_maps_geo` | 地址转经纬度（地理编码） |
| `mcp_amap_maps_regeocode` | 经纬度转地址（逆地理编码） |
| `mcp_amap_maps_ip_location` | IP定位 |
| `mcp_amap_maps_weather` | 查询城市天气 |
| `mcp_amap_maps_text_search` | 关键词POI搜索 |
| `mcp_amap_maps_around_search` | 周边POI搜索 |
| `mcp_amap_maps_search_detail` | POI详情查询 |
| `mcp_amap_maps_direction_driving` | 驾车路径规划 |
| `mcp_amap_maps_direction_walking` | 步行路径规划 |
| `mcp_amap_maps_direction_transit_integrated` | 公交综合路径规划 |
| `mcp_amap_maps_bicycling` | 骑行路径规划 |
| `mcp_amap_maps_distance` | 距离测量 |

---

## 5. stock-quote — 行情报价

**工具数量**: 21 | **状态**: 🟢 enabled

A股/港股/美股/期货/外汇行情报价及K线数据。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_stock_quote_A___` | A股实时报价 |
| `mcp_stock_quote_A_K_` | A股K线数据 |
| `mcp_stock_quote_A_K___` | A股K线复权数据 |
| `mcp_stock_quote_____` | 美股报价 |
| `mcp_stock_quote___K_` | 美股K线 |
| `mcp_stock_quote_____K_` | 全球指数K线 |
| `mcp_stock_quote_______` | 外盘期货报价/合约 |
| `mcp_stock_quote_____` | 美股排行 |

---

## 6. minimax — 音视频/图像生成

**工具数量**: 9 | **状态**: 🟢 enabled

MiniMax大模型服务，支持文本生成图片、视频、音乐、语音。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_minimax_text_to_image` | 文本生成图片 |
| `mcp_minimax_generate_video` | 文本/图片生成视频 |
| `mcp_minimax_query_video_generation` | 查询视频生成状态 |
| `mcp_minimax_music_generation` | AI音乐生成 |
| `mcp_minimax_text_to_audio` | 文本转语音 |
| `mcp_minimax_play_audio` | 播放音频文件 |
| `mcp_minimax_list_voices` | 列出可用音色 |
| `mcp_minimax_voice_clone` | 克隆声音 |
| `mcp_minimax_voice_design` | AI设计音色 |

---

## 7. github — GitHub操作

**工具数量**: 26 | **状态**: 🟢 enabled

GitHub仓库、Issue、PR、文件操作。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_github_create_repository` | 创建仓库 |
| `mcp_github_fork_repository` | Fork仓库 |
| `mcp_github_get_file_contents` | 获取文件内容 |
| `mcp_github_create_or_update_file` | 创建/更新单文件 |
| `mcp_github_push_files` | 批量推送文件 |
| `mcp_github_list_commits` | 列出提交记录 |
| `mcp_github_create_branch` | 创建分支 |
| `mcp_github_search_repositories` | 搜索仓库 |
| `mcp_github_search_code` | 搜索代码 |
| `mcp_github_search_issues` | 搜索Issue/PR |
| `mcp_github_search_users` | 搜索用户 |
| `mcp_github_create_issue` | 创建Issue |
| `mcp_github_get_issue` | 获取Issue详情 |
| `mcp_github_update_issue` | 更新Issue |
| `mcp_github_add_issue_comment` | 添加Issue评论 |
| `mcp_github_list_issues` | 列出Issue |
| `mcp_github_create_pull_request` | 创建PR |
| `mcp_github_get_pull_request` | 获取PR详情 |
| `mcp_github_list_pull_requests` | 列出PR |
| `mcp_github_create_pull_request_review` | 创建PR Review |
| `mcp_github_merge_pull_request` | 合并PR |
| `mcp_github_get_pull_request_files` | 获取PR变更文件 |
| `mcp_github_get_pull_request_status` | 获取PR CI状态 |
| `mcp_github_get_pull_request_comments` | 获取PR评论 |
| `mcp_github_get_pull_request_reviews` | 获取PR Reviews |
| `mcp_github_update_pull_request_branch` | 更新PR分支 |

---

## 8. doc-forge — 文档处理

**工具数量**: 16 | **状态**: 🟢 enabled

文档格式转换、读取、编辑、比对。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_doc_forge_document_reader` | 读取文档（PDF/DOCX/TXT/HTML/CSV） |
| `mcp_doc_forge_pdf_merger` | 合并PDF |
| `mcp_doc_forge_pdf_splitter` | 拆分PDF |
| `mcp_doc_forge_docx_to_pdf` | DOCX转PDF |
| `mcp_doc_forge_docx_to_html` | DOCX转HTML |
| `mcp_doc_forge_html_to_markdown` | HTML转Markdown |
| `mcp_doc_forge_html_to_text` | HTML转纯文本 |
| `mcp_doc_forge_html_cleaner` | 清理HTML |
| `mcp_doc_forge_html_formatter` | 格式化HTML |
| `mcp_doc_forge_html_extract_resources` | 提取HTML资源 |
| `mcp_doc_forge_excel_read` | 读取Excel文件 |
| `mcp_doc_forge_format_convert` | 文档格式转换 |
| `mcp_doc_forge_text_diff` | 文本比对 |
| `mcp_doc_forge_text_splitter` | 文本分割 |
| `mcp_doc_forge_text_formatter` | 文本格式化 |
| `mcp_doc_forge_text_encoding_converter` | 文本编码转换 |

---

## 9. excel — Excel操作

**工具数量**: 6 | **状态**: 🟢 enabled

Excel工作表读写、格式化、创建表格。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_excel_excel_read_sheet` | 读取Excel工作表 |
| `mcp_excel_excel_write_to_sheet` | 写入Excel工作表 |
| `mcp_excel_excel_describe_sheets` | 列出工作表信息 |
| `mcp_excel_excel_format_range` | 格式化单元格 |
| `mcp_excel_excel_create_table` | 创建Excel表格 |
| `mcp_excel_excel_copy_sheet` | 复制工作表 |

---

## 10. playwright — 浏览器自动化

**工具数量**: 8 | **状态**: 🟢 enabled

浏览器自动化测试和网页抓取。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_playwright_navigate` | 导航到URL |
| `mcp_playwright_screenshot` | 截图 |
| `mcp_playwright_get_page_content` | 获取页面HTML |
| `mcp_playwright_get_text` | 获取元素文本 |
| `mcp_playwright_click` | 点击元素 |
| `mcp_playwright_fill` | 填写表单 |
| `mcp_playwright_wait_for_selector` | 等待元素出现 |
| `mcp_playwright_close_browser` | 关闭浏览器 |

---

## 11. pandoc — 文档格式转换

**工具数量**: 1 | **状态**: 🟢 enabled

支持Markdown、HTML、PDF、DOCX、RST、LaTeX、EPUB等格式互转。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_pandoc_convert_contents` | 文档格式转换 |

---

## 12. sqlite — SQLite数据库

**工具数量**: 5 | **状态**: 🟢 enabled

本地SQLite数据库操作。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_sqlite_list_tables` | 列出所有表 |
| `mcp_sqlite_describe_table` | 查看表结构 |
| `mcp_sqlite_read_query` | 执行SELECT查询 |
| `mcp_sqlite_write_query` | 执行INSERT/UPDATE/DELETE |
| `mcp_sqlite_create_table` | 创建表 |

---

## 13. weather — 天气预报

**工具数量**: 3 | **状态**: 🟢 enabled

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_weather_get_weather` | 获取当前天气 |
| `mcp_weather_get_forecast` | 获取天气预报（1-5天） |
| `mcp_weather_get_air_quality` | 获取空气质量 |

---

## 14. openscad — 3D建模

**工具数量**: 7 | **状态**: 🟢 enabled

自然语言生成3D模型，支持导出STL等多种格式。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_openscad_create_3d_model` | 从描述创建3D模型 |
| `mcp_openscad_modify_3d_model` | 修改3D模型 |
| `mcp_openscad_export_model` | 导出3D模型 |
| `mcp_openscad_list_models` | 列出已有模型 |
| `mcp_openscad_get_supported_3d_shapes` | 获取支持的形状类型 |
| `mcp_openscad_generate_image` | 文本生成图片（Venice.ai） |
| `mcp_openscad_generate_image_gemini` | 文本生成图片（Gemini） |

---

## 15. vision-mcp — 图像理解

**工具数量**: 1 | **状态**: 🟢 enabled

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_vision_mcp_analyze_image` | 分析图片内容并提供详细描述 |

---

## 16. gezhe — PPT生成

**工具数量**: 1 | **状态**: 🟢 enabled

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_gezhe_generate_ppt_by_topic` | 根据主题生成PPT演示文稿 |

---

## 17. how-to-cook — 菜谱查询

**工具数量**: 5 | **状态**: 🟢 enabled

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_howtocook_getAllRecipes` | 获取所有菜谱 |
| `mcp_howtocook_getRecipesByCategory` | 按分类查询菜谱 |
| `mcp_howtocook_getRecipeById` | 查询指定菜谱详情 |
| `mcp_howtocook_whatToEat` | 不知道吃什么，随机推荐 |
| `mcp_howtocook_recommendMeals` | 根据忌口智能推荐一周膳食计划 |

---

## 18. 其他工具

### bmi-mcp — BMI计算

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_bmi_mcp______` | 根据身高体重计算BMI并给出健康建议 |

### bw-ir — 发票验真

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_bw_ir_invoice_verification` | 验证发票真实性，支持增值税发票，普通发票等多种票据 |

### food-detective — 美食推荐

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_food_detective______` | 传入地名，返回当地5条美食和推荐理由 |

### qrcode-mcp — 二维码生成

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_qrcode_mcp______` | 生成二维码图片（PNG/JPG/GIF） |

### market-cmapi — 地区新闻

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_market_cmapi_______` | 查询指定省市区的本地新闻 |
| `mcp_market_cmapi__________` | 查询支持的新闻地区列表 |

### local_time — 本地时间

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_local_time_get_current_time` | 获取当前本地时间 |

---

## 已禁用 / 连接失败的MCP

| MCP名称 | 状态 | 说明 |
|---------|------|------|
| luckin | 🔴 disabled | 瑞幸咖啡MCP |
| mbti | 🔴 disabled | MBTI人格测试MCP |
| mmb-mcp | ❌ failed | 慢慢买MCP，401认证失败 |
| xhs-toolkit | ❌ failed | 小红书MCP，连接超时 |
| xhs-toolkit-http | ❌ failed | 小红书HTTP服务，本地服务未启动 |

---

> 📌 本文档由 Hermes Agent 自动生成，每8小时更新一次
> 📅 更新日期：2026年06月26日 08:02 CST
