# Hermes Agent MCP API 文档

> 🤖 Powered by Hermes Agent | 更新日期：2026年06月23日 08:01 CST
>
> ⚠️ 状态说明 | 🟢 enabled = 已启用 | 🔴 disabled = 已禁用 | ❌ failed = 连接失败

---

## MCP 服务总览（27个已启用 / 3个已禁用或失败）

| 状态 | 数量 | MCP名称 |
|----------|------|---------|
| 🟢 enabled | 27 | antv-chart, antv-visual, bmi-mcp, bw-ir, didi, food-detective, how-to-cook, market-cmapi, openscad, vision-mcp, gezhe, playwright, pandoc, doc-forge, excel, minimax, qrcode-mcp, stock-quote, amap, github, sqlite, weather, local_time |
| 🔴 disabled | 2 | luckin, mbti |
| ❌ failed | 1 | mmb-mcp (401认证失败), xhs-toolkit (超时), xhs-toolkit-http (服务未启动) |

---

## 1. 金融数据（antv-chart / antv-visual）

**MCP名称**: antv-chart, antv-visual  
**功能描述**: A股/基金/指数/债券/宏观经济数据查询，包含财务指标、分红、估值、机构持仓等完整金融数据API。

### 股票数据（Stock）

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_chart_list_stock_all` | 获取全市场A股/B股股票基本信息列表 |
| `mcp_antv_chart_get_stock_basic_info` | 查询股票基本信息（名称、板块、上市状态等） |
| `mcp_antv_chart_list_stock_industries` | 查询股票所属申万行业分类 |
| `mcp_antv_chart_list_stock_balance_sheet` | 查询股票资产负债表数据 |
| `mcp_antv_chart_list_stock_income_statements` | 查询股票利润表数据 |
| `mcp_antv_chart_list_stk_income_state_pit` | 查询股票利润表数据（时点版） |
| `mcp_antv_chart_list_stk_balan_sheet_pit` | 查询股票资产负债表数据（时点版） |
| `mcp_antv_chart_list_stock_cash_flows` | 查询股票现金流量表数据 |
| `mcp_antv_chart_list_stock_cash_flows_pit` | 查询股票现金流量表数据（时点版） |
| `mcp_antv_chart_list_stock_adjusted_quotes` | 查询股票复权行情数据 |
| `mcp_antv_chart_list_stock_unadjusted_quotes` | 查询股票未复权行情数据 |
| `mcp_antv_chart_list_stock_industries` | 查询股票行业分类信息 |
| `mcp_antv_chart_list_stock_margin_securities` | 查询融资融券标的证券 |
| `mcp_antv_chart_list_stock_earnings_bulletins` | 查询业绩快报数据 |
| `mcp_antv_chart_list_stocks_dividends` | 查询股票分红派息信息 |
| `mcp_antv_chart_list_stock_share_adj_factors` | 查询股票除权除息事件 |
| `mcp_antv_chart_list_stock_capital_changes` | 查询公司股本变动历史 |
| `mcp_antv_chart_list_stock_holder_cnt` | 查询股东户数及持股结构 |
| `mcp_antv_chart_list_stock_top10_circulating_shareh` | 查询前十大流通股东 |
| `mcp_antv_chart_list_stock_management_dirs` | 查询管理层人员信息 |
| `mcp_antv_chart_list_stock_core_mgmt_changes` | 查询核心管理层变更记录 |
| `mcp_antv_chart_list_stock_institutional_holdings_stats` | 查询机构持股统计 |
| `mcp_antv_chart_list_stock_executive_shareholding_change` | 查询高管持股变动 |
| `mcp_antv_chart_list_stock_special_notices` | 查询股票特别提示信息 |
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
| `mcp_antv_chart_list_stock_rights_issues` | 查询配股发行信息 |
| `mcp_antv_chart_get_stock_former_names` | 查询股票历史曾用名 |
| `mcp_antv_chart_get_company_profiles` | 查询公司基本信息 |

### 基金数据（Fund）

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_chart_list_fund_all` | 获取全市场基金列表 |
| `mcp_antv_chart_get_fund_basic_info` | 查询基金基本信息 |
| `mcp_antv_chart_get_fund_categories` | 查询基金三级分类体系 |
| `mcp_antv_chart_list_fund_nav_history` | 查询基金历史净值数据 |
| `mcp_antv_chart_list_fund_adj_navs` | 查询基金复权单位净值 |
| `mcp_antv_chart_list_fund_daily_quotes` | 查询基金日行情数据 |
| `mcp_antv_chart_list_fund_adj_quotes` | 查询基金前复权日行情 |
| `mcp_antv_chart_list_fund_return_rate` | 查询基金历史回报率 |
| `mcp_antv_chart_list_fund_fee_structures` | 查询基金详细费率信息 |
| `mcp_antv_chart_list_fund_dividend_distributions` | 查询基金分红信息 |
| `mcp_antv_chart_list_fund_share_splits` | 查询基金份额拆分与折算 |
| `mcp_antv_chart_list_fund_shares` | 查询基金份额变动明细 |
| `mcp_antv_chart_list_fund_fin_inds` | 查询基金主要财务指标 |
| `mcp_antv_chart_list_fund_fin_inds_q` | 查询基金季度主要财务指标 |
| `mcp_antv_chart_get_fund_manager_basic_info` | 查询基金经理基本信息 |
| `mcp_antv_chart_get_fund_award_records` | 查询基金所获奖项信息 |
| `mcp_antv_chart_get_fund_code_assoc` | 查询基金关联关系 |
| `mcp_antv_chart_list_fund_listings_record` | 查询基金的发行与上市信息 |
| `mcp_antv_chart_list_fund_portfolio_stock_holdings` | 查询基金持仓股票信息 |
| `mcp_antv_chart_list_fund_portfolio_bond_holdings` | 查询基金持仓债券信息 |
| `mcp_antv_chart_list_fund_portfolio_asset_holdings` | 查询基金资产配置详情 |
| `mcp_antv_chart_list_portfolio_fund_holdings` | 查询基金的持仓基金数据 |
| `mcp_antv_chart_list_fund_hold_industry` | 查询持有特定行业的基金 |
| `mcp_antv_chart_list_industry_hold_fund` | 查询持有特定行业股票的基金 |
| `mcp_antv_chart_list_concept_hold_fund` | 查询持有特定概念的基金列表 |
| `mcp_antv_chart_list_etf_constituent_stks` | 查询ETF成分股信息 |
| `mcp_antv_chart_list_etf_sub_red_lists` | 查询ETF申购赎回清单 |
| `mcp_antv_chart_list_fund_hold_structures` | 查询基金持有人结构 |
| `mcp_antv_chart_list_fund_invest_targets` | 查询基金投资标的配置 |
| `mcp_antv_chart_list_fund_perf_benchmarks` | 查询基金业绩比较基准 |
| `mcp_antv_chart_list_subscription_redemption_status` | 查询基金申购赎回状态 |
| `mcp_antv_chart_list_currency_yield_history` | 查询货币基金收益历史 |

### 指数数据（Index）

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_chart_get_index_basic_info` | 查询指数基本信息 |
| `mcp_antv_chart_list_index_quotes` | 查询指数历史日行情 |
| `mcp_antv_chart_list_index_quote_barch` | 批量查询指数历史行情 |
| `mcp_antv_chart_list_perf_benchmark_quote` | 查询基准指数历史行情 |

### 宏观经济（Macro）

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_chart_list_economic_cn_cpi` | 查询中国CPI居民消费价格指数 |
| `mcp_antv_chart_list_economic_cn_ppi` | 查询中国PPI工业生产者出厂价格指数 |
| `mcp_antv_chart_list_money_supplies` | 查询货币供应量数据（M0/M1/M2） |
| `mcp_antv_chart_list_gover_bond_yield` | 查询国债收益率曲线数据 |
| `mcp_antv_chart_list_money_market_repo_in` | 查询国债收益率曲线（货币市场版） |
| `mcp_antv_chart_list_social_financing_sto` | 查询社会融资规模存量数据 |
| `mcp_antv_chart_list_trade_special_date` | 查询A股交易日衍生日期 |
| `mcp_antv_chart_is_trade_date` | 判断是否为交易日 |
| `mcp_antv_chart_get_cn_trade_calender_list` | 获取A股市场交易日列表 |

### 图表可视化（antv-visual）

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_visual_generate_line_chart` | 生成折线图（趋势/时间序列） |
| `mcp_antv_visual_generate_bar_chart` | 生成水平柱状图（分类对比） |
| `mcp_antv_visual_generate_column_chart` | 生成柱状图（分类对比） |
| `mcp_antv_visual_generate_pie_chart` | 生成饼图（比例展示） |
| `mcp_antv_visual_generate_area_chart` | 生成面积图（趋势+总量） |
| `mcp_antv_visual_generate_scatter_chart` | 生成散点图（相关性分析） |
| `mcp_antv_visual_generate_boxplot_chart` | 生成箱线图（数据分布） |
| `mcp_antv_visual_generate_violin_chart` | 生成小提琴图（数据分布） |
| `mcp_antv_visual_generate_histogram_chart` | 生成直方图（频率分布） |
| `mcp_antv_visual_generate_dual_axes_chart` | 生成双轴图（趋势+对比） |
| `mcp_antv_visual_generate_treemap_chart` | 生成矩形树图（层级数据） |
| `mcp_antv_visual_generate_word_cloud_chart` | 生成词云图（文本频率） |
| `mcp_antv_visual_generate_radar_chart` | 生成雷达图（多维对比） |
| `mcp_antv_visual_generate_funnel_chart` | 生成漏斗图（转化流程） |
| `mcp_antv_visual_generate_sankey_chart` | 生成桑基图（数据流向） |
| `mcp_antv_visual_generate_network_graph` | 生成网络图（关系网络） |
| `mcp_antv_visual_generate_organization_chart` | 生成组织架构图 |
| `mcp_antv_visual_generate_mind_map` | 生成思维导图 |
| `mcp_antv_visual_generate_fishbone_diagram` | 生成鱼骨图（因果分析） |
| `mcp_antv_visual_generate_flow_diagram` | 生成流程图 |
| `mcp_antv_visual_generate_liquid_chart` | 生成水球图/仪表盘 |
| `mcp_antv_visual_generate_venn_chart` | 生成韦恩图（集合关系） |
| `mcp_antv_visual_generate_district_map` | 生成区域分布地图（中国） |
| `mcp_antv_visual_generate_path_map` | 生成路线图（旅游路线） |
| `mcp_antv_visual_generate_pin_map` | 生成点标注地图（POI分布） |

### 搜索与资源

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_chart_search` | 金融产品搜索（股票/基金/ETF/港股/行业/概念） |
| `mcp_antv_chart_list_industries` | 查询行业列表 |
| `mcp_antv_chart_list_concepts` | 查询概念板块列表 |
| `mcp_antv_chart_list_hk_stock_dividends` | 查询港股分红派息信息 |
| `mcp_antv_chart_list_report_institutions` | 查询研究机构列表 |
| `mcp_antv_chart_list_resources` | 列出antv-chart可用资源 |
| `mcp_antv_chart_list_prompts` | 列出antv-chart可用提示模板 |
| `mcp_antv_chart_get_prompt` | 获取指定提示模板 |

### 图表生成API（Base64图片）

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_antv_chart_generate_chart` | 将ECharts配置转换为Base64图片 |

---

## 2. 地图出行（高德地图 amap）

**MCP名称**: amap  
**功能描述**: 高德地图Web服务API，支持地理编码、地点搜索、路径规划、天气查询。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_amap_maps_geo` | 地址/地名 → 经纬度坐标（地理编码） |
| `mcp_amap_maps_regeocode` | 经纬度坐标 → 行政区划地址（逆地理编码） |
| `mcp_amap_maps_text_search` | 关键词搜索POI地点 |
| `mcp_amap_maps_around_search` | 周边地点搜索（半径范围POI） |
| `mcp_amap_maps_search_detail` | 查询POI详细信息 |
| `mcp_amap_maps_direction_driving` | 驾车路径规划 |
| `mcp_amap_maps_direction_walking` | 步行路径规划 |
| `mcp_amap_maps_direction_transit_integrated` | 公交综合路径规划 |
| `mcp_amap_maps_bicycling` | 骑行路径规划 |
| `mcp_amap_maps_distance` | 距离测量（驾车/步行/直线） |
| `mcp_amap_maps_weather` | 查询城市天气预报 |
| `mcp_amap_maps_ip_location` | IP地址定位 |

---

## 3. 滴滴出行（didi）

**MCP名称**: didi  
**功能描述**: 滴滴出行API，支持车型预估、打车下单、订单查询、司机位置追踪。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_didi_taxi_estimate` | 查看网约车车型及预估价格 |
| `mcp_didi_taxi_create_order` | 创建打车订单（直接发单） |
| `mcp_didi_taxi_query_order` | 查询打车订单状态和司机信息 |
| `mcp_didi_taxi_get_driver_location` | 获取司机实时位置 |
| `mcp_didi_taxi_cancel_order` | 取消打车订单 |
| `mcp_didi_taxi_generate_ride_app_link` | 生成App深度链接 |
| `mcp_didi_maps_textsearch` | 搜索POI地点（滴滴地图） |
| `mcp_didi_maps_place_around` | 周边地点搜索（滴滴地图） |
| `mcp_didi_maps_regeocode` | 经纬度→地址（滴滴地图） |
| `mcp_didi_maps_direction_driving` | 驾车路径规划（滴滴地图） |
| `mcp_didi_maps_direction_walking` | 步行路径规划（滴滴地图） |
| `mcp_didi_maps_direction_transit` | 公交路径规划（滴滴地图） |
| `mcp_didi_maps_direction_bicycling` | 骑行路径规划（滴滴地图） |

---

## 4. 股票行情（stock-quote）

**MCP名称**: stock-quote  
**功能描述**: A股/美股/全球指数实时行情和K线数据。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_stock_quote_A___` | A股实时报价（多品种） |
| `mcp_stock_quote_A_K_` | A股K线数据（1分钟~月K） |
| `mcp_stock_quote_A_K___` | A股K线复权数据（前复权/后复权） |
| `mcp_stock_quote___K_` | 美股K线数据 |
| `mcp_stock_quote_____K_` | 全球指数K线数据 |
| `mcp_stock_quote_______` | 外盘期货合约数据 |
| `mcp_stock_quote_____` | 美股排行（涨跌幅/成交量/市值排序） |

---

## 5. 天气（weather）

**MCP名称**: weather  
**功能描述**: 天气预报和空气质量查询。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_weather_get_weather` | 获取当前天气实况 |
| `mcp_weather_get_forecast` | 获取天气预报（1-5天） |
| `mcp_weather_get_air_quality` | 获取空气质量（AQI/PM2.5等） |

---

## 6. GitHub 操作（github）

**MCP名称**: github  
**功能描述**: GitHub API操作，支持仓库/Issue/PR/代码/用户搜索等完整GitHub操作。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_github_get_file_contents` | 获取仓库文件/目录内容 |
| `mcp_github_list_commits` | 列出仓库提交记录 |
| `mcp_github_list_pull_requests` | 列出Pull Request列表 |
| `mcp_github_get_pull_request` | 获取PR详情 |
| `mcp_github_get_pull_request_files` | 获取PR变更文件列表 |
| `mcp_github_get_pull_request_reviews` | 获取PR审查意见 |
| `mcp_github_get_pull_request_comments` | 获取PR评论 |
| `mcp_github_get_pull_request_status` | 获取PR CI/CD状态 |
| `mcp_github_create_pull_request` | 创建Pull Request |
| `mcp_github_create_pull_request_review` | 提交PR审查意见 |
| `mcp_github_merge_pull_request` | 合并Pull Request |
| `mcp_github_update_pull_request_branch` | 更新PR分支 |
| `mcp_github_list_issues` | 列出Issue列表 |
| `mcp_github_get_issue` | 获取Issue详情 |
| `mcp_github_create_issue` | 创建Issue |
| `mcp_github_update_issue` | 更新Issue状态/内容 |
| `mcp_github_add_issue_comment` | 添加Issue评论 |
| `mcp_github_search_repositories` | 搜索GitHub仓库 |
| `mcp_github_search_issues` | 搜索Issue和PR |
| `mcp_github_search_code` | 搜索代码 |
| `mcp_github_search_users` | 搜索GitHub用户 |
| `mcp_github_create_branch` | 创建分支 |
| `mcp_github_create_or_update_file` | 创建/更新单个文件 |
| `mcp_github_push_files` | 批量推送多个文件 |
| `mcp_github_create_repository` | 创建新仓库 |
| `mcp_github_fork_repository` | Fork仓库 |

---

## 7. 文件处理（pandoc / doc-forge）

**MCP名称**: pandoc, doc-forge  
**功能描述**: 文档格式转换、文本处理、PDF操作。

### Pandoc转换

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_pandoc_convert_contents` | 文档格式转换（Markdown↔HTML↔PDF↔DOCX等） |

### DocForge文档工具

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_doc_forge_document_reader` | 读取文档内容（PDF/DOCX/TXT/HTML/CSV） |
| `mcp_doc_forge_format_convert` | 文档格式互转（Markdown/HTML/XML/JSON） |
| `mcp_doc_forge_html_to_markdown` | HTML转Markdown |
| `mcp_doc_forge_html_to_text` | HTML转纯文本 |
| `mcp_doc_forge_docx_to_html` | DOCX转HTML |
| `mcp_doc_forge_docx_to_pdf` | DOCX转PDF |
| `mcp_doc_forge_text_encoding_converter` | 文本编码转换 |
| `mcp_doc_forge_text_formatter` | 格式化文本（缩进/行距） |
| `mcp_doc_forge_text_splitter` | 文本分割（按行数或分隔符） |
| `mcp_doc_forge_text_diff` | 文本差异对比 |
| `mcp_doc_forge_html_formatter` | HTML格式化/美化 |
| `mcp_doc_forge_html_cleaner` | 清理HTML冗余标签 |
| `mcp_doc_forge_html_extract_resources` | 提取HTML中的资源 |
| `mcp_doc_forge_pdf_merger` | 合并多个PDF |
| `mcp_doc_forge_pdf_splitter` | 拆分PDF文件 |

---

## 8. Excel操作（excel）

**MCP名称**: excel  
**功能描述**: Excel文件读取、写入、格式化、表格创建。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_excel_excel_read_sheet` | 读取Excel工作表数据 |
| `mcp_excel_excel_write_to_sheet` | 写入数据到Excel工作表 |
| `mcp_excel_excel_describe_sheets` | 列出工作表信息 |
| `mcp_excel_excel_format_range` | 格式化单元格区域（字体/颜色/边框） |
| `mcp_excel_excel_create_table` | 创建Excel表格 |
| `mcp_excel_excel_copy_sheet` | 复制工作表 |

---

## 9. MiniMax AI（minimax）

**MCP名称**: minimax  
**功能描述**: MiniMax大模型API，支持图片生成、视频生成、语音合成、音乐生成。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_minimax_text_to_image` | 文字生成图片 |
| `mcp_minimax_generate_video` | 文字/图片生成视频 |
| `mcp_minimax_query_video_generation` | 查询视频生成任务状态 |
| `mcp_minimax_text_to_audio` | 文字转语音（TTS） |
| `mcp_minimax_music_generation` | AI音乐生成（歌词+风格→音乐） |
| `mcp_minimax_voice_clone` | 语音克隆 |
| `mcp_minimax_voice_design` | 语音设计（描述→声音） |
| `mcp_minimax_list_voices` | 列出可用音色 |
| `mcp_minimax_play_audio` | 播放音频文件 |
| `mcp_minimax_list_prompts` | 列出可用提示模板 |
| `mcp_minimax_get_prompt` | 获取指定提示模板 |
| `mcp_minimax_list_resources` | 列出可用资源 |
| `mcp_minimax_read_resource` | 读取指定资源 |

---

## 10. 视觉理解（vision-mcp）

**MCP名称**: vision-mcp  
**功能描述**: 多模态AI图片/视频理解，支持GLM-4V视觉模型。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_vision_mcp_analyze_image` | 分析图片内容（OCR/物体识别/场景理解） |

---

## 11. 3D建模（openscad）

**MCP名称**: openscad  
**功能描述**: 一句话说需求→生成3D模型并导出STL文件。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_openscad_create_3d_model` | 根据自然语言描述创建3D模型 |
| `mcp_openscad_modify_3d_model` | 修改现有3D模型 |
| `mcp_openscad_export_model` | 导出3D模型（STL等格式） |
| `mcp_openscad_list_models` | 列出已生成的3D模型 |
| `mcp_openscad_get_supported_3d_shapes` | 获取支持的3D形状类型 |
| `mcp_openscad_generate_image` | Venice.ai图片生成 |
| `mcp_openscad_generate_image_gemini` | Google Gemini图片生成 |
| `mcp_openscad_list_prompts` | 列出可用提示模板 |
| `mcp_openscad_get_prompt` | 获取指定提示模板 |
| `mcp_openscad_list_resources` | 列出可用资源 |
| `mcp_openscad_read_resource` | 读取指定资源 |

---

## 12. 浏览器自动化（playwright）

**MCP名称**: playwright  
**功能描述**: Playwright浏览器自动化，支持网页截图/点击/填表/导航。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_playwright_navigate` | 导航到指定URL |
| `mcp_playwright_screenshot` | 截图 |
| `mcp_playwright_click` | 点击元素 |
| `mcp_playwright_fill` | 填写表单字段 |
| `mcp_playwright_get_text` | 获取元素文本内容 |
| `mcp_playwright_get_page_content` | 获取页面HTML内容 |
| `mcp_playwright_wait_for_selector` | 等待元素出现 |
| `mcp_playwright_close_browser` | 关闭浏览器 |
| `mcp_playwright_list_prompts` | 列出可用提示模板 |
| `mcp_playwright_get_prompt` | 获取指定提示模板 |
| `mcp_playwright_list_resources` | 列出可用资源 |
| `mcp_playwright_read_resource` | 读取指定资源 |

---

## 13. 本地时间（local_time）

**MCP名称**: local_time  
**功能描述**: 获取当前本地时间。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_local_time_get_current_time` | 获取当前本地时间 |

---

## 14. SQLite数据库（sqlite）

**MCP名称**: sqlite  
**功能描述**: 本地SQLite数据库操作，支持创建表/读写数据。

| 工具名称 | 功能说明 |
|---------|---------|
| `mcp_sqlite_create_table` | 创建数据库表 |
| `mcp_sqlite_read_query` | 执行SELECT查询 |
| `mcp_sqlite_write_query` | 执行INSERT/UPDATE/DELETE |
| `mcp_sqlite_describe_table` | 查看表结构 |
| `mcp_sqlite_list_tables` | 列出所有表 |

---

## 15. 其他工具

| 工具名称 | MCP名称 | 功能说明 |
|---------|---------|---------|
| `mcp_bmi_mcp______` | bmi-mcp | BMI体重指数计算与健康建议 |
| `mcp_bw_ir_invoice_verification` | bw-ir | 发票真伪验证（增值税发票等） |
| `mcp_food_detective______` | food-detective | 地方美食推荐（输入城市→5道美食） |
| `mcp_gezhe_generate_ppt_by_topic` | gezhe | 根据主题生成PPT |
| `mcp_qrcode_mcp______` | qrcode-mcp | 本地二维码生成（文本/URL→PNG） |
| `mcp_market_cmapi_______` | market-cmapi | 中国区域新闻查询 |
| `mcp_market_cmapi__________` | market-cmapi | 查询支持的省市区域 |
| `mcp_how-to-cook______` | how-to-cook | 中餐菜谱查询（美食杰API） |

---

## 工具统计

| 类别 | 工具数量 |
|------|---------|
| 金融数据（antv-chart）| ~100+ |
| 图表可视化（antv-visual）| 26 |
| 地图/出行（amap + didi）| 18 |
| 股票行情（stock-quote）| 7 |
| 天气（weather）| 3 |
| GitHub（github）| 25 |
| 文件处理（pandoc/doc-forge）| 16 |
| Excel（excel）| 6 |
| MiniMax AI（minimax）| 11 |
| 视觉理解（vision-mcp）| 1 |
| 3D建模（openscad）| 9 |
| 浏览器自动化（playwright）| 9 |
| 本地时间（local_time）| 1 |
| SQLite数据库（sqlite）| 5 |
| 其他工具 | 9 |
| **总计** | **~240+** |

---

> 📅 文档更新时间：2026年06月23日 08:01 CST  
> 🤖 由 Hermes Agent 自动生成
