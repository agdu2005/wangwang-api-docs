# WangWang Agent - MCP API 文档

> 更新日期：2026-06-15

---

## 📊 数据查询类

### antv-chart（股票/基金/指数/宏观数据）| 124个工具

| 工具名 | 功能说明 |
|--------|---------|
| list_stock_all | 获取全市场A股和B股股票基本信息 |
| list_fund_all | 获取全市场基金列表 |
| get_stock_basic_info | 查询股票基本信息 |
| get_company_profiles | 查询公司详细信息 |
| get_stock_industries | 查询股票所属行业分类 |
| search | 按关键字搜索股票/基金/ETF/港股/行业/概念 |
| list_stock_adjusted_quotes | 查询股票复权行情数据 |
| list_stock_unadjusted_quotes | 查询股票未复权行情数据 |
| list_stock_share_adj_factors | 查询历史除权除息事件 |
| list_index_quotes | 查询指数历史行情 |
| list_index_quote_barch | 批量查询指数行情 |
| get_index_basic_info | 查询指数基本信息 |
| list_stock_income_statements | 查询股票利润表 |
| list_stock_balance_sheet | 查询股票资产负债表 |
| list_stock_cash_flows | 查询股票现金流量表 |
| list_stk_income_state_pit | 查询股票利润表(时点) |
| list_stk_balan_sheet_pit | 查询股票资产负债表(时点) |
| list_stock_cash_flows_pit | 查询股票现金流量表(时点) |
| list_stock_earnings_bulletins | 查询业绩快报数据 |
| list_stock_holder_cnt | 查询股东户数及持股结构 |
| list_stock_capital_changes | 查询股本变动历史 |
| list_stock_management_dirs | 查询管理层人员信息 |
| list_stock_core_mgmt_changes | 查询核心管理层变更记录 |
| list_stock_related_transactions | 查询关联交易详情 |
| list_stock_major_contracts | 查询重大合同公告 |
| list_stock_special_notices | 查询特别提示信息 |
| list_stock_executive_shareholding_change | 查询高管持股变动 |
| list_stock_pledge_details | 查询股权质押明细 |
| list_stock_freeze_details | 查询股权冻结明细 |
| list_stock_tender_offers | 查询要约收购事件 |
| list_stock_absorption_mergers | 查询吸收合并事件 |
| list_stock_offerings | 查询增发方案详情 |
| list_stocks_public_offering_place | 查询公开增发/配售结果 |
| get_stock_rights_issues | 查询配股发行信息 |
| list_stocks_rights_issue_res | 查询配股发行结果 |
| list_stock_repurchase_plans | 查询股份回购计划 |
| list_stock_institutional_holdings_stats | 查询机构持股统计数据 |
| list_stock_top10_circulating_shareh | 查询十大流通股东 |
| list_stock_earnings_bulletins | 查询业绩快报 |
| get_stock_former_names | 查询股票历史曾用名 |
| get_stock_margin_securities | 查询融资融券标的证券 |
| list_report_schema | 查询定期报告预披露日程 |
| list_fund_nav_history | 查询基金历史净值 |
| list_fund_daily_quotes | 查询基金日行情数据 |
| list_fund_adj_quotes | 查询基金前复权行情 |
| list_fund_adj_navs | 查询基金复权单位净值 |
| list_fund_return_rate | 查询基金历史回报率 |
| list_fund_hold_stock_holdings | 查询基金持仓股票 |
| list_fund_portfolio_stock_holdings | 查询基金持仓股票详情 |
| list_fund_portfolio_bond_holdings | 查询基金持仓债券 |
| list_fund_portfolio_asset_holdings | 查询基金资产配置详情 |
| list_fund_portfolio_fund_holdings | 查询基金持仓基金 |
| list_fund_hold_industry | 查询持有某行业的基金 |
| list_industry_hold_fund | 查询持有某行业股票的基金 |
| list_concept_hold_fund | 查询持有某概念的基金列表 |
| list_fund_hold_structures | 查询基金持有人结构 |
| list_fund_shares | 查询基金份额变动明细 |
| list_fund_share_splits | 查询基金份额拆分与折算 |
| list_fund_dividend_distributions | 查询基金分红信息 |
| list_etf_constituent_stks | 查询ETF成分股信息 |
| list_etf_sub_red_lists | 查询ETF申购赎回清单 |
| get_fund_basic_info | 查询基金基本信息 |
| get_fund_categories | 查询基金三级分类体系 |
| get_fund_manager_basic_info | 查询基金经理基本信息 |
| list_fund_invest_targets | 查询基金投资标的 |
| list_fund_perf_benchmarks | 查询基金业绩比较基准 |
| list_fund_fee_structures | 查询基金费率信息 |
| get_fund_award_records | 查询基金所获奖项 |
| get_fund_code_assoc | 查询基金关联关系 |
| get_fund_listings_record | 查询基金发行上市信息 |
| list_fund_fin_inds | 查询基金主要财务指标 |
| list_fund_fin_inds_q | 查询基金季度财务指标 |
| list_currency_yield_history | 查询货币基金收益 |
| list_hk_stock_dividends | 查询港股分红派息 |
| list_concepts | 查询概念列表 |
| get_cn_trade_calendar_list | 查询A股交易日列表 |
| is_trade_date | 判断是否为交易日 |
| get_trade_special_date | 查询交易日衍生日期 |
| list_economic_cn_cpi | 查询中国CPI历史数据 |
| list_economic_cn_ppi | 查询中国PPI历史数据 |
| list_money_supplies | 查询货币供应量数据 |
| list_gover_bond_yield | 查询国债收益率曲线 |
| list_money_market_repo_in | 查询货币市场数据 |
| list_social_financing_sto | 查询社会融资规模存量 |
| generate_chart | 将ECharts配置转换为Base64图片 |
| generate_nex_chart | 生成图表图片 |

---

### antv-visual（图表可视化）| 25个工具

| 工具名 | 功能说明 |
|--------|---------|
| generate_line_chart | 生成折线图，展示数据趋势 |
| generate_column_chart | 生成柱状图，比较分类数据 |
| generate_bar_chart | 生成横向条形图 |
| generate_pie_chart | 生成饼图，展示比例构成 |
| generate_area_chart | 生成面积图，展示连续数据趋势 |
| generate_scatter_chart | 生成散点图，展示变量关系 |
| generate_histogram_chart | 生成直方图，展示频率分布 |
| generate_boxplot_chart | 生成箱线图，展示统计摘要 |
| generate_violin_chart | 生成小提琴图，展示数据分布 |
| generate_radar_chart | 生成雷达图，展示多维数据 |
| generate_sankey_chart | 生成桑基图，展示数据流动 |
| generate_funnel_chart | 生成漏斗图，展示转化漏斗 |
| generate_treemap_chart | 生成矩形树图，展示层级数据 |
| generate_venn_chart | 生成韦恩图，展示集合关系 |
| generate_word_cloud_chart | 生成词云图，展示词频权重 |
| generate_liquid_chart | 生成水球图，展示百分比数值 |
| generate_mind_map | 生成思维导图，展示层级结构 |
| generate_organization_chart | 生成组织结构图 |
| generate_flow_diagram | 生成流程图，展示步骤决策 |
| generate_network_graph | 生成网络图，展示关系网络 |
| generate_fishbone_diagram | 生成鱼骨图，展示因果分析 |
| generate_dual_axes_chart | 生成双轴图，折线+柱状组合 |
| generate_district_map | 生成区域分布地图（中国） |
| generate_path_map | 生成路线地图，展示路线规划 |
| generate_pin_map | 生成点位地图，展示POI分布 |

---

### stock-quote（行情报价）| 21个工具

| 工具名 | 功能说明 |
|--------|---------|
| A股报价 | A股实时行情报价 |
| A股K线 | A股K线数据 |
| A股K线复权 | A股复权K线数据 |
| A股排行 | A股涨跌幅/成交量/换手率等排名 |
| 港股报价 | 港股实时行情 |
| 港股K线 | 港股K线数据 |
| 港股排行 | 港股涨跌幅排名 |
| 美股报价 | 美股实时行情 |
| 美股K线 | 美股K线数据 |
| 美股排行 | 美股涨跌幅排名 |
| 美股品种 | 美股品种信息 |
| 全球指数报价 | 全球指数实时行情 |
| 全球指数K线 | 全球指数K线 |
| 外汇报价 | 外汇实时报价 |
| 外汇K线 | 外汇K线数据 |
| 内盘期货报价 | 内盘期货实时行情 |
| 内盘期货K线 | 内盘期货K线 |
| 内盘期货合约 | 内盘期货合约信息 |
| 外盘期货报价 | 外盘期货实时行情 |
| 外盘期货K线 | 外盘期货K线 |
| 外盘期货合约 | 外盘期货合约信息 |

---

### amap（高德地图）| 12个工具

| 工具名 | 功能说明 |
|--------|---------|
| maps_geo | 地址转经纬度（地理编码） |
| maps_regeocode | 经纬度转行政区划地址 |
| maps_ip_location | IP地址定位 |
| maps_weather | 查询城市天气 |
| maps_text_search | 关键词搜索POI地点 |
| maps_around_search | 周边POI搜索 |
| maps_search_detail | 查询POI详细信息 |
| maps_direction_driving | 驾车路径规划 |
| maps_direction_walking | 步行路径规划 |
| maps_direction_bicycling | 骑行路径规划 |
| maps_direction_transit_integrated | 公交综合路线规划 |
| maps_distance | 距离测量（驾车/步行/球面） |

---

### didi（滴滴出行）| 13个工具

| 工具名 | 功能说明 |
|--------|---------|
| maps_textsearch | 搜索POI地点信息 |
| maps_regeocode | 经纬度转地址 |
| maps_place_around | 周边地点搜索 |
| maps_direction_driving | 驾车路线规划 |
| maps_direction_transit | 公交路线规划 |
| maps_direction_walking | 步行路线规划 |
| maps_direction_bicycling | 骑行路线规划 |
| taxi_estimate | 查看网约车车型和预估价格 |
| taxi_create_order | 直接创建打车订单 |
| taxi_query_order | 查询打车订单状态 |
| taxi_cancel_order | 取消打车订单 |
| taxi_get_driver_location | 获取司机实时位置 |
| taxi_generate_ride_app_link | 生成跳转APP/小程序的深度链接 |

---

### market-cmapi（新闻查询）| 2个工具

| 工具名 | 功能说明 |
|--------|---------|
| 查询地区新闻 | 中国各省市区域新闻查询 |
| 查询支持的新闻地区 | 查询支持新闻的省市地区 |

---

### weather（天气）| 3个工具

| 工具名 | 功能说明 |
|--------|---------|
| get_weather | 获取当前天气 |
| get_forecast | 获取天气预报（1-5天） |
| get_air_quality | 获取空气质量 |

---

### local_time（时间）| 1个工具

| 工具名 | 功能说明 |
|--------|---------|
| get_current_time | 获取当前本地时间 |

---

## 🎨 内容生成类

### minimax（音视频生成）| 9个工具

| 工具名 | 功能说明 |
|--------|---------|
| text_to_image | 文字生成图片 |
| generate_video | 文字/图片生成视频 |
| text_to_audio | 文字转语音音频 |
| music_generation | AI音乐生成 |
| voice_clone | 声音克隆 |
| voice_design | 根据描述生成声音 |
| list_voices | 列出可用音色列表 |
| play_audio | 播放音频文件 |
| query_video_generation | 查询视频生成任务状态 |

---

### openscad（3D建模/图像）| 7个工具

| 工具名 | 功能说明 |
|--------|---------|
| create_3d_model | 自然语言创建3D模型 |
| modify_3d_model | 修改现有3D模型 |
| export_model | 导出3D模型（STL等格式） |
| list_models | 列出已生成的3D模型 |
| generate_image | Venice.ai图像生成 |
| generate_image_gemini | Google Gemini图像生成 |
| get_supported_3d_shapes | 获取支持的3D形状类型 |

---

### gezhe（PPT生成）| 1个工具

| 工具名 | 功能说明 |
|--------|---------|
| generate_ppt_by_topic | 根据主题生成PPT演示文稿 |

---

### qrcode-mcp（二维码）| 1个工具

| 工具名 | 功能说明 |
|--------|---------|
| 二维码生成 | 生成二维码图片 |

---

## 📄 文档处理类

### doc-forge（文档处理）| 16个工具

| 工具名 | 功能说明 |
|--------|---------|
| document_reader | 读取PDF/DOCX/TXT/HTML/CSV文档 |
| pdf_merger | 合并多个PDF文件 |
| pdf_splitter | 拆分PDF文件 |
| docx_to_pdf | Word转PDF |
| docx_to_html | Word转HTML |
| html_to_text | HTML转纯文本 |
| html_to_markdown | HTML转Markdown |
| html_cleaner | 清理HTML标签属性 |
| html_formatter | 格式化/美化HTML代码 |
| html_extract_resources | 提取HTML中的资源 |
| text_diff | 比较两个文本文件差异 |
| text_splitter | 按分隔符/行数拆分文本 |
| text_formatter | 格式化文本（缩进/行距） |
| text_encoding_converter | 文本编码转换 |
| excel_read | 读取Excel文件转为JSON |
| format_convert | 文档格式互转 |

---

### excel（Excel操作）| 6个工具

| 工具名 | 功能说明 |
|--------|---------|
| excel_read_sheet | 读取Excel工作表数据 |
| excel_write_to_sheet | 写入数据到Excel工作表 |
| excel_format_range | 格式化单元格样式 |
| excel_create_table | 创建Excel表格 |
| excel_describe_sheets | 列出所有工作表信息 |
| excel_copy_sheet | 复制工作表 |

---

### pandoc（格式转换）| 1个工具

| 工具名 | 功能说明 |
|--------|---------|
| convert-contents | 在Markdown/HTML/PDF/DOCX/RST/LaTeX等格式间转换 |

---

## 🖥️ 浏览器自动化

### playwright（浏览器自动化）| 8个工具

| 工具名 | 功能说明 |
|--------|---------|
| navigate | 导航到指定URL |
| screenshot | 截取页面截图 |
| get_page_content | 获取页面完整HTML内容 |
| get_text | 获取元素文本内容 |
| click | 点击页面元素 |
| fill | 填写表单字段 |
| wait_for_selector | 等待元素出现 |
| close_browser | 关闭浏览器 |

---

## 🗄️ 数据存储类

### sqlite（本地数据库）| 5个工具

| 工具名 | 功能说明 |
|--------|---------|
| read_query | 执行SELECT查询 |
| write_query | 执行INSERT/UPDATE/DELETE |
| create_table | 创建新表 |
| list_tables | 列出所有表 |
| describe_table | 获取表结构信息 |

---

## 🔧 开发工具类

### github（GitHub操作）| 26个工具

| 工具名 | 功能说明 |
|--------|---------|
| search_repositories | 搜索GitHub仓库 |
| search_code | 搜索代码 |
| search_issues | 搜索Issue和PR |
| search_users | 搜索GitHub用户 |
| get_file_contents | 获取文件/目录内容 |
| create_repository | 创建新仓库 |
| fork_repository | Fork仓库 |
| push_files | 批量推送文件 |
| create_or_update_file | 创建或更新单个文件 |
| create_branch | 创建分支 |
| list_commits | 获取提交记录 |
| create_issue | 创建Issue |
| get_issue | 获取Issue详情 |
| list_issues | 列出仓库Issue |
| update_issue | 更新Issue |
| add_issue_comment | 添加Issue评论 |
| create_pull_request | 创建Pull Request |
| get_pull_request | 获取PR详情 |
| list_pull_requests | 列出仓库PR |
| create_pull_request_review | 创建PR审查 |
| merge_pull_request | 合并PR |
| get_pull_request_files | 获取PR变更文件 |
| get_pull_request_status | 获取PR CI状态 |
| get_pull_request_comments | 获取PR评论 |
| get_pull_request_reviews | 获取PR审查意见 |
| update_pull_request_branch | 更新PR分支 |

---

## 🍳 生活服务类

### how-to-cook（菜谱）| 5个工具

| 工具名 | 功能说明 |
|--------|---------|
| mcp_howtocook_whatToEat | 根据人数推荐菜品组合 |
| mcp_howtocook_recommendMeals | 智能推荐一周膳食计划 |
| mcp_howtocook_getRecipesByCategory | 按分类查询菜谱（水产/早餐/荤菜/素菜等） |
| mcp_howtocook_getRecipeById | 查询指定菜谱详情（食材/步骤） |
| mcp_howtocook_getAllRecipes | 获取所有菜谱 |

---

### food-detective（美食推荐）| 1个工具

| 工具名 | 功能说明 |
|--------|---------|
| 推荐美食 | 传入地名，返回5条当地美食及推荐理由 |

---

### bmi-mcp（健康）| 1个工具

| 工具名 | 功能说明 |
|--------|---------|
| BMI体重指数 | 根据身高体重计算BMI，返回健康评估和建议 |

---

## 🧾 发票与工具类

### bw-ir（发票验证）| 1个工具

| 工具名 | 功能说明 |
|--------|---------|
| invoice_verification | 验证发票真实性，支持增值税发票/普通发票/电子发票等14类票据核验 |

---

## 🔍 视觉识别类

### vision-mcp（图像理解）| 1个工具

| 工具名 | 功能说明 |
|--------|---------|
| analyze_image | 分析图片内容并提供详细描述 |

---

## ❌ 不可用/失败

| MCP名称 | 状态 |
|---------|------|
| luckin | ✗ disabled（已禁用） |
| mbti | ✗ disabled（已禁用） |
| gf-windmill | ✗ disabled（已禁用） |
| mmb-mcp | ✗ 连接失败（401未授权） |
| xhs-toolkit | ✗ 连接失败（超时） |
| xhs-toolkit-http | ✗ 连接失败（本地服务未启动） |

---

> 📝 共收录 **27个** MCP服务，约 **300+** 个工具函数
> 
> 由 Hermes Agent 自动生成 | WangWang API Docs
