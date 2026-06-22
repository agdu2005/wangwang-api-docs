# Hermes Agent MCP API 文档

> 🤖 Powered by Hermes Agent | 更新日期：2026年06月22日 08:14 CST
>
> ⚠️ 状态说明 | 🟢 enabled = 已启用 | 🔴 disabled = 已禁用 | ❌ failed = 连接失败

---

## MCP 服务总览（24个已启用 / 4个已禁用或失败）

| 状态 | 数量 | MCP名称 |
|----------|------|---------|
| 🟢 enabled | 24 | antv-chart, antv-visual, bmi-mcp, bw-ir, didi, food-detective, how-to-cook, market-cmapi, openscad, vision-mcp, gezhe, playwright, pandoc, doc-forge, excel, minimax, qrcode-mcp, stock-quote, amap, github, sqlite, weather, local_time |
| 🔴 disabled | 2 | luckin, mbti |
| ❌ failed | 2 | mmb-mcp (401认证失败), xhs-toolkit/xhs-toolkit-http (连接超时/拒绝) |

---

## 🟢 antv-chart（金融数据）

**传输层**: HTTPS | **工具数**: 124 | **状态**: 🟢 已连接

金融数据API，支持A股、基金、指数、港股、宏观经济数据查询与分析。

### 股票数据
| 工具名 | 功能说明 |
|--------|----------|
| list_stock_all | 获取全市场A股/B股股票基本信息列表 |
| get_stock_basic_info | 通过股票代码查询沪深京A股/B股详细基本信息 |
| get_stock_former_names | 查询股票历史曾用名信息 |
| list_stock_adjusted_quotes | 查询股票复权行情数据 |
| list_stock_unadjusted_quotes | 查询股票未复权行情数据 |
| list_stock_share_adj_factors | 查询股票历史除权除息事件详情 |
| get_company_profiles | 查询股票所属公司基本信息 |
| list_stock_income_statements | 查询股票利润表数据 |
| list_stock_balance_sheet | 查询股票资产负债表数据 |
| list_stock_cash_flows | 查询股票现金流量表数据 |
| list_stock_earnings_bulletins | 查询股票业绩快报数据 |
| list_stock_report_schema | 查询股票定期报告预披露日程 |
| list_stock_holder_cnt | 查询股东户数及持股结构数据 |
| list_stock_major_contracts | 查询上市公司重大合同公告详情 |
| list_stock_management_dirs | 查询上市公司管理层人员名录 |
| list_stock_core_mgmt_changes | 查询核心管理层历史变更记录 |
| list_stock_executive_shareholding_change | 查询高管持股变动明细 |
| list_stock_capital_changes | 查询公司股本变动历史 |
| list_stock_pledge_details | 查询股权质押明细数据 |
| list_stock_freeze_details | 查询股权冻结明细数据 |
| list_stock_institutional_holdings_stats | 查询机构持股统计数据 |
| list_stock_top10_circulating_shareh | 查询十大流通股东信息 |
| list_stock_offerings | 查询股票增发方案详情 |
| get_stock_rights_issues | 查询股票配股发行信息 |
| list_stock_tender_offers | 查询要约收购事件详情 |
| list_stock_repurchase_plans | 查询股份回购计划信息 |
| list_stock_related_transactions | 查询关联交易详细信息 |
| list_stock_absorption_mergers | 查询吸收合并事件详情 |
| list_stock_special_notices | 查询股票特别提示信息 |
| get_stock_industries | 查询股票所属行业分类（申万） |
| get_stock_margin_securities | 查询融资融券标的证券信息 |

### 基金数据
| 工具名 | 功能说明 |
|--------|----------|
| list_fund_all | 获取全市场基金列表 |
| get_fund_basic_info | 查询基金基本信息 |
| get_fund_categories | 查询基金三级分类体系 |
| list_fund_nav_history | 查询基金历史净值数据 |
| list_fund_adj_navs | 查询基金复权单位净值数据 |
| list_fund_daily_quotes | 查询基金历史日行情数据 |
| list_fund_adj_quotes | 查询基金前复权日行情数据 |
| list_fund_return_rate | 查询基金历史回报率数据 |
| list_fund_fin_inds | 查询基金主要财务指标 |
| list_fund_fin_inds_q | 查询基金季度主要财务指标 |
| list_fund_perf_benchmarks | 查询基金业绩比较基准配置详情 |
| list_perf_benchmark_quote | 查询基金业绩比较基准历史行情 |
| list_fund_invest_targets | 查询基金投资标的及配置比例 |
| list_fund_portfolio_stock_holdings | 查询基金持仓股票信息 |
| list_fund_portfolio_bond_holdings | 查询基金持仓债券配置信息 |
| list_fund_portfolio_asset_holdings | 查询基金资产配置详情 |
| list_portfolio_fund_holdings | 查询基金持仓基金数据 |
| list_fund_hold_industry | 查询持有指定行业股票的基金 |
| list_industry_hold_fund | 查询持有指定行业股票的基金 |
| list_concept_hold_fund | 查询持有指定概念板块的基金 |
| get_fund_code_assoc | 查询基金与其他基金的历史关联 |
| get_fund_listings_record | 查询基金发行与上市信息 |
| get_fund_manager_basic_info | 查询基金经理基本信息和任职情况 |
| list_fund_share_splits | 查询基金份额拆分与折算历史 |
| list_fund_dividend_distributions | 查询基金分红信息 |
| list_fund_fee_structures | 查询基金详细费率信息 |
| list_fund_hold_structures | 查询基金持有人结构信息 |
| list_fund_shares | 查询基金份额变动明细 |
| get_fund_award_records | 查询基金所获奖项信息 |
| list_subscription_redemption_status | 查询基金申购赎回状态变更 |
| list_etf_constituent_stks | 查询ETF成分股信息 |
| list_etf_sub_red_lists | 查询ETF申购赎回清单基本信息 |
| list_currency_yield_history | 查询货币基金收益情况 |

### 指数数据
| 工具名 | 功能说明 |
|--------|----------|
| get_index_basic_info | 查询指数基本信息 |
| list_index_quotes | 查询指数历史日行情数据 |
| list_index_quote_barch | 查询指数历史日行情（批量） |
| search | 通过关键字搜索金融产品（A股/基金/ETF/港股/行业/概念） |

### 港股数据
| 工具名 | 功能说明 |
|--------|----------|
| list_hk_stock_dividends | 查询港股分红派息信息 |

### 宏观经济数据
| 工具名 | 功能说明 |
|--------|----------|
| list_economic_cn_cpi | 查询中国CPI历史数据 |
| list_economic_cn_ppi | 查询中国PPI历史数据 |
| list_money_supplies | 查询中国货币供应量数据 |
| list_gover_bond_yield | 查询中国国债收益率曲线 |
| list_money_market_repo_in | 查询货币市场数据 |
| list_social_financing_sto | 查询中国社会融资规模存量数据 |

### 交易日历
| 工具名 | 功能说明 |
|--------|----------|
| get_cn_trade_calender_list | 返回A股市场交易日列表 |
| get_trade_special_date | 返回交易日衍生日期 |
| is_trade_date | 判断是否为交易日 |

### 股票发行数据
| 工具名 | 功能说明 |
|--------|----------|
| list_stocks_dividends | 查询股票分红派息详细信息 |
| list_stocks_public_offering_place | 查询公开增发或配售结果 |
| list_stocks_rights_issue_res | 查询配股发行结果 |
| list_report_institutions | 查询研究机构列表 |

### 图表生成
| 工具名 | 功能说明 |
|--------|----------|
| generate_chart | 将ECharts配置转换为Base64图片 |
| generate_nex_chart | 生成图表图片（带标识符） |

---

## 🟢 antv-visual（可视化图表）

**传输层**: HTTPS | **工具数**: 25 | **状态**: 🟢 已连接

AI图表生成工具，支持25种图表类型的可视化生成。

| 工具名 | 功能说明 |
|--------|----------|
| generate_line_chart | 生成折线图，展示数据趋势随时间变化 |
| generate_area_chart | 生成面积图，展示连续变量数据趋势 |
| generate_bar_chart | 生成水平条形图，用于数值比较 |
| generate_column_chart | 生成柱状图，用于分类数据比较 |
| generate_pie_chart | 生成饼图，展示各部分占比 |
| generate_scatter_chart | 生成散点图，展示两变量关系 |
| generate_boxplot_chart | 生成箱线图，展示数据统计分布 |
| generate_violin_chart | 生成小提琴图，展示数据分布 |
| generate_histogram_chart | 生成直方图，展示数据频率分布 |
| generate_radar_chart | 生成雷达图，展示多维数据 |
| generate_heatmap_chart | 生成热力图（可用散点图模拟） |
| generate_polar_chart | 生成极坐标图 |
| generate_sankey_chart | 生成桑基图，展示数据流转 |
| generate_funnel_chart | 生成漏斗图，展示转化率 |
| generate_mind_map | 生成思维导图，展示层次结构 |
| generate_organization_chart | 生成组织架构图 |
| generate_flow_diagram | 生成流程图，展示步骤与决策点 |
| generate_network_graph | 生成网络关系图 |
| generate_treemap_chart | 生成矩形树图，展示层次数据 |
| generate_fishbone_diagram | 生成鱼骨图，分析因果关系 |
| generate_district_map | 生成区域分布地图（中国行政区划） |
| generate_path_map | 生成路线地图，展示行程路线 |
| generate_pin_map | 生成地点标注地图 |
| generate_liquid_chart | 生成水球图，展示百分比指标 |
| generate_word_cloud_chart | 生成词云图，展示词频权重 |

---

## 🟢 bmi-mcp（健康指数）

**传输层**: HTTPS | **工具数**: 1 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| BMI体重指数 | 根据身高、体重查询BMI指数，返回健康评估、提示与建议 |

---

## 🟢 bw-ir（发票验证）

**传输层**: HTTPS | **工具数**: 1 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| invoice_verification | 验证发票真实性与合规性，支持增值税专用发票、普通发票、电子发票等14类票据 |

---

## 🟢 didi（滴滴出行）

**传输层**: HTTPS | **工具数**: 13 | **状态**: 🟢 已连接

滴滴出行服务，包含地图导航与打车功能。

### 地图导航
| 工具名 | 功能说明 |
|--------|----------|
| maps_direction_driving | 驾车路径规划 |
| maps_direction_bicycling | 骑行路径规划 |
| maps_direction_walking | 步行路径规划 |
| maps_direction_transit | 综合公交/地铁通勤方案 |
| maps_textsearch | 关键词搜索POI地点信息 |
| maps_place_around | 周边地点搜索 |
| maps_regeocode | 经纬度坐标转地址信息 |

### 打车服务
| 工具名 | 功能说明 |
|--------|----------|
| taxi_estimate | 查询网约车预估价格与车型 |
| taxi_create_order | 创建打车订单 |
| taxi_query_order | 查询订单状态、司机信息 |
| taxi_cancel_order | 取消打车订单 |
| taxi_get_driver_location | 获取司机实时位置 |
| taxi_generate_ride_app_link | 生成跳转App/小程序的深度链接 |

---

## 🟢 food-detective（美食推荐）

**传输层**: HTTPS | **工具数**: 1 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| 推荐美食 | 传入地名，返回5条当地美食和推荐理由 |

---

## 🟢 how-to-cook（菜谱查询）

**传输层**: HTTPS | **工具数**: 5 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| mcp_howtocook_getAllRecipes | 获取所有菜谱 |
| mcp_howtocook_getRecipesByCategory | 按分类查询菜谱（水产/早餐/甜品/饮品/荤菜/素菜等） |
| mcp_howtocook_getRecipeById | 查询指定菜谱的完整详情（食材+步骤） |
| mcp_howtocook_whatToEat | 根据人数推荐适合的菜品组合 |
| mcp_howtocook_recommendMeals | 智能推荐一周膳食计划与购物清单 |

---

## 🟢 market-cmapi（新闻资讯）

**传输层**: HTTPS | **工具数**: 2 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| 查询地区新闻 | 按省市区域查询新闻资讯 |
| 查询支持的新闻地区 | 查询API支持的省市区域列表 |

---

## 🟢 openscad（3D建模）

**传输层**: stdio | **工具数**: 7 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| create_3d_model | 通过自然语言描述生成3D模型 |
| modify_3d_model | 修改已有3D模型 |
| export_model | 导出3D模型（STL等格式） |
| list_models | 列出所有已生成的3D模型 |
| get_supported_3d_shapes | 获取支持的3D形状类型 |
| generate_image | 使用Venice.ai生成图片 |
| generate_image_gemini | 使用Google Gemini生成图片 |

---

## 🟢 vision-mcp（视觉理解）

**传输层**: stdio | **工具数**: 1 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| analyze_image | 分析图片内容并提供详细描述，支持物体识别/OCR/场景理解 |

---

## 🟢 gezhe（PPT生成）

**传输层**: HTTPS | **工具数**: 1 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| generate_ppt_by_topic | 根据主题生成PPT演示文稿 |

---

## 🟢 playwright（浏览器自动化）

**传输层**: stdio | **工具数**: 8 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| navigate | 导航到指定URL |
| screenshot | 截取当前页面截图 |
| get_page_content | 获取页面完整HTML内容 |
| get_text | 获取元素文本内容 |
| click | 点击页面元素 |
| fill | 填写表单字段 |
| wait_for_selector | 等待元素出现 |
| close_browser | 关闭浏览器 |

---

## 🟢 pandoc（文档格式转换）

**传输层**: stdio | **工具数**: 1 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| convert-contents | 在多种文档格式间转换（Markdown/HTML/PDF/DOCX/RST/LaTeX/EPUB/TXT/IPYNB） |

---

## 🟢 doc-forge（文档处理）

**传输层**: stdio | **工具数**: 16 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| document_reader | 读取PDF/DOCX/TXT/HTML/CSV文档内容 |
| pdf_merger | 合并多个PDF文件 |
| pdf_splitter | 拆分PDF为多个文件 |
| docx_to_pdf | DOCX转PDF格式 |
| docx_to_html | DOCX转HTML |
| html_cleaner | 清理HTML无效标签和属性 |
| html_to_text | HTML转纯文本 |
| html_to_markdown | HTML转Markdown |
| html_extract_resources | 提取HTML中的图片/视频/链接资源 |
| html_formatter | 格式化美化HTML代码 |
| text_diff | 对比两个文本文件差异 |
| text_splitter | 按分隔符或行数拆分文本文件 |
| text_formatter | 格式化文本（缩进/行距） |
| text_encoding_converter | 文本编码转换（UTF-8/BIG5/GBK等） |
| excel_read | 读取Excel文件并转为JSON |
| format_convert | 文档格式互转（Markdown/HTML/XML/JSON） |

---

## 🟢 excel（Excel操作）

**传输层**: stdio | **工具数**: 6 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| excel_read_sheet | 读取Excel工作表数据（支持分页） |
| excel_write_to_sheet | 向Excel工作表写入数据 |
| excel_describe_sheets | 列出所有工作表信息 |
| excel_create_table | 创建Excel表格 |
| excel_copy_sheet | 复制工作表到新表 |
| excel_format_range | 设置单元格样式（字体/颜色/边框/数字格式） |

---

## 🟢 minimax（AI多媒体）

**传输层**: stdio | **工具数**: 9 | **状态**: 🟢 已连接

MiniMax AI多媒体生成服务，支持语音、视频、图片、音乐。

| 工具名 | 功能说明 |
|--------|----------|
| text_to_audio | 文本转语音（支持多种音色/语速/音调/情绪） |
| list_voices | 列出所有可用音色 |
| voice_clone | 克隆音色 |
| play_audio | 播放音频文件（WAV/MP3） |
| text_to_image | 根据提示词生成图片 |
| generate_video | 根据提示词生成视频 |
| query_video_generation | 查询视频生成任务状态 |
| music_generation | 根据歌词和风格生成音乐 |
| voice_design | 根据描述生成自定义音色 |

---

## 🟢 qrcode-mcp（二维码）

**传输层**: HTTPS | **工具数**: 1 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| 二维码生成 | 将文本/URL生成为二维码图片，支持多种尺寸和格式 |

---

## 🟢 stock-quote（行情数据）

**传输层**: HTTPS | **工具数**: 21 | **状态**: 🟢 已连接

实时行情数据，支持A股、港股、美股、期货、外汇、全球指数。

| 工具名 | 功能说明 |
|--------|----------|
| A股报价 | A股实时行情报价 |
| A股K线 | A股K线数据（支持多周期） |
| A股K线复权 | A股复权K线数据（前复权/后复权） |
| A股排行 | A股排行榜（涨跌幅/成交额/市值） |
| 港股报价 | 港股实时行情报价 |
| 港股K线 | 港股K线数据 |
| 美股报价 | 美股实时行情报价 |
| 美股K线 | 美股K线数据 |
| 美股排行 | 美股排行榜 |
| 美股品种 | 美股品种列表 |
| 全球指数报价 | 全球主要指数实时报价 |
| 全球指数K线 | 全球指数K线数据 |
| 外盘期货报价 | 外盘期货实时报价 |
| 外盘期货K线 | 外盘期货K线数据 |
| 外盘期货合约 | 外盘期货合约信息 |
| 内盘期货报价 | 内盘期货实时报价 |
| 内盘期货K线 | 内盘期货K线数据 |
| 内盘期货合约 | 内盘期货合约信息 |
| 外汇报价 | 外汇实时报价 |
| 外汇K线 | 外汇K线数据 |

---

## 🟢 amap（高德地图）

**传输层**: stdio | **工具数**: 12 | **状态**: 🟢 已连接

高德地图服务，包含地理编码、路径规划、天气查询。

| 工具名 | 功能说明 |
|--------|----------|
| maps_geo | 地址/地标解析为经纬度坐标 |
| maps_regeocode | 经纬度坐标转行政区划地址 |
| maps_ip_location | IP地址定位 |
| maps_weather | 查询城市天气 |
| maps_text_search | 关键词搜索POI |
| maps_around_search | 周边地点搜索 |
| maps_search_detail | 查询POI详细信息 |
| maps_direction_driving | 驾车路径规划 |
| maps_direction_walking | 步行路径规划 |
| maps_direction_transit_integrated | 综合公交/地铁/火车通勤方案 |
| maps_bicycling | 骑行路径规划 |
| maps_distance | 两点间距离测量（驾车/步行/球面） |

---

## 🟢 github（GitHub操作）

**传输层**: stdio | **工具数**: 26 | **状态**: 🟢 已连接

GitHub仓库管理、PR、Issue操作。

### 仓库管理
| 工具名 | 功能说明 |
|--------|----------|
| create_repository | 创建新仓库 |
| fork_repository | Fork仓库 |
| get_file_contents | 获取文件/目录内容 |
| push_files | 批量推送多个文件 |
| create_or_update_file | 创建或更新单个文件 |
| list_commits | 获取分支提交记录 |
| create_branch | 创建新分支 |

### Issue操作
| 工具名 | 功能说明 |
|--------|----------|
| create_issue | 创建Issue |
| update_issue | 更新Issue（状态/标签/指派） |
| get_issue | 获取Issue详情 |
| list_issues | 列出Issue（支持过滤） |
| add_issue_comment | 添加Issue评论 |

### Pull Request操作
| 工具名 | 功能说明 |
|--------|----------|
| create_pull_request | 创建PR |
| list_pull_requests | 列出PR（支持过滤） |
| get_pull_request | 获取PR详情 |
| merge_pull_request | 合并PR |
| create_pull_request_review | 创建PR Review |
| get_pull_request_files | 获取PR变更文件列表 |
| get_pull_request_status | 获取PR CI状态 |
| get_pull_request_comments | 获取PR评论 |
| get_pull_request_reviews | 获取PR Reviews |
| update_pull_request_branch | 用最新代码更新PR分支 |

### 搜索
| 工具名 | 功能说明 |
|--------|----------|
| search_repositories | 搜索仓库 |
| search_code | 搜索代码 |
| search_issues | 搜索Issue和PR |
| search_users | 搜索用户 |

---

## 🟢 sqlite（数据库）

**传输层**: stdio | **工具数**: 5 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| list_tables | 列出所有数据表 |
| describe_table | 获取表结构信息 |
| read_query | 执行SELECT查询 |
| write_query | 执行INSERT/UPDATE/DELETE |
| create_table | 创建新数据表 |

---

## 🟢 weather（天气预报）

**传输层**: stdio | **工具数**: 3 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| get_weather | 获取当前天气 |
| get_forecast | 获取天气预报（支持1-5天） |
| get_air_quality | 获取空气质量（AQI/PM2.5等） |

---

## 🟢 local_time（本地时间）

**传输层**: stdio | **工具数**: 1 | **状态**: 🟢 已连接

| 工具名 | 功能说明 |
|--------|----------|
| get_current_time | 获取当前本地时间 |

---

## 🔴 luckin（瑞幸咖啡）— 已禁用

---

## 🔴 mbti（MBTI测试）— 已禁用

---

## ❌ mmb-mcp（慢慢买）— 连接失败（401认证失败）

---

## ❌ xhs-toolkit / xhs-toolkit-http（小红书）— 连接失败（超时/连接拒绝）

---

## 🔴 gf-windmill（gf-windmill）— 已禁用

---

*本文档由Hermes Agent自动生成并定时更新*
