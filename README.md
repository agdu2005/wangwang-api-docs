# Hermes Agent MCP API 文档

> 更新日期：2026年06月20日
> Hermes Agent 版本：最新版
> 北京时间：2026年06月20日 08:02

---

## 📋 MCP 服务总览

| 状态 | 说明 |
|------|------|
| ✅ enabled | 已启用且正常连接 |
| ❌ disabled | 已禁用 |
| ⚠️ failed | 已启用但连接失败 |

**统计**：共 30 个 MCP 服务，26 个已启用，其中 22 个正常连接。

---

## 1. antv-chart（A股金融数据）

**功能**：沪深京A股/港股/美股行情查询，基金信息，财务数据，宏观经济数据。

**工具列表**（共 124 个）：

| 工具名 | 功能 |
|--------|------|
| list_stock_all | 获取全市场A股和B股股票基本信息列表 |
| list_fund_all | 获取全市场基金列表，支持分页查询 |
| get_stock_basic_info | 通过股票代码查询沪深京市场A股、B股详细基本信息 |
| get_company_profiles | 查询股票所属公司的基本信息 |
| list_concepts | 获取概念板块列表 |
| list_industries | 查询行业列表，支持模糊匹配 |
| get_stock_industries | 根据股票代码查询申万行业分类 |
| list_index_quote_barch | 查询指数行情数据 |
| list_index_quotes | 查询指数历史日行情 |
| list_stock_unadjusted_quotes | 查询股票未复权行情数据 |
| list_stock_adjusted_quotes | 查询股票复权行情数据 |
| list_stock_share_adj_factors | 查询历史除权除息事件 |
| list_stk_income_state_pit | 查询利润表（时点）数据 |
| list_stk_balan_sheet_pit | 查询资产负债表数据 |
| list_stock_cash_flows_pit | 查询现金流量表数据 |
| list_stock_income_statements | 查询利润详情 |
| list_stock_balance_sheet | 查询资产负债表 |
| list_stock_cash_flows | 查询现金流量数据 |
| list_stock_earnings_bulletins | 查询业绩快报数据 |
| list_stock_special_notices | 查询特别提示信息 |
| get_trade_special_date | 返回交易日衍生日期 |
| get_cn_trade_calender_list | 返回指定周期内的A股交易日列表 |
| list_stocks_dividends | 查询分红派息详细信息 |
| list_stock_offerings | 查询增发方案详情 |
| list_stocks_rights_issue_res | 查询配股发行结果 |
| get_stock_rights_issues | 查询配股发行信息 |
| list_stock_capital_changes | 查询公司股本变动历史 |
| list_stock_pledge_details | 查询股权质押明细 |
| list_stock_freeze_details | 查询股权冻结明细 |
| list_stock_repurchase_plans | 查询股份回购计划 |
| list_stock_tender_offers | 查询要约收购事件 |
| list_stock_absorption_mergers | 查询吸收合并事件 |
| list_stock_major_contracts | 查询重大合同公告 |
| list_stock_top10_circulating_shareh | 查询历史十大流通股东 |
| list_stock_executive_shareholding_change | 查询高管持股变动 |
| list_stock_holder_cnt | 查询股东户数及持股结构 |
| list_stock_management_dirs | 查询管理层历史信息 |
| list_stock_core_mgmt_changes | 查询核心管理层变更 |
| list_stock_related_transactions | 查询关联交易详情 |
| list_stock_institutional_holdings_stats | 查询机构持股统计数据 |
| list_stock_report_schema | 查询定期报告预披露日程 |
| get_stock_margin_securities | 查询融资融券标的证券 |
| get_stock_former_names | 查询股票历史曾用名 |
| list_fund_hold_industry | 查询持有指定行业的基金 |
| list_fund_nav_history | 查询基金历史净值 |
| list_fund_adj_navs | 查询基金复权净值 |
| list_fund_return_rate | 查询基金历史回报率 |
| list_fund_daily_quotes | 查询基金日行情数据 |
| list_fund_adj_quotes | 查询基金前复权日行情 |
| list_currency_yield_history | 查询货币基金收益 |
| list_fund_perf_benchmarks | 查询基金业绩比较基准 |
| list_fund_fee_structures | 查询基金费率信息 |
| list_fund_invest_targets | 查询基金投资标的 |
| list_subscription_redemption_status | 查询基金申购赎回状态 |
| get_fund_basic_info | 查询基金基本信息 |
| get_fund_manager_basic_info | 查询基金经理信息 |
| get_fund_code_assoc | 查询基金关联关系 |
| get_fund_listings_record | 查询基金发行上市信息 |
| get_fund_categories | 查询基金分类体系 |
| get_fund_award_records | 查询基金所获奖项 |
| list_report_institutions | 查询研究机构列表 |

---

## 2. antv-visual（图表可视化）

**功能**：通过自然语言生成各类图表（折线图、饼图、地图、流程图等）。

**工具列表**（共 25 个）：

| 工具名 | 功能 |
|--------|------|
| generate_line_chart | 生成折线图，展示时间趋势 |
| generate_bar_chart | 生成水平条形图 |
| generate_column_chart | 生成柱状图，对比分类数据 |
| generate_pie_chart | 生成饼图，展示比例构成 |
| generate_area_chart | 生成面积图，展示趋势 |
| generate_scatter_chart | 生成散点图，展示变量关系 |
| generate_funnel_chart | 生成漏斗图，展示转化流程 |
| generate_radar_chart | 生成雷达图，展示多维数据 |
| generate_sankey_chart | 生成桑基图，展示数据流向 |
| generate_histogram_chart | 生成直方图，展示频率分布 |
| generate_boxplot_chart | 生成箱线图，统计摘要 |
| generate_violin_chart | 生成小提琴图，展示分布 |
| generate_treemap_chart | 生成矩形树图，展示层次数据 |
| generate_mind_map | 生成思维导图 |
| generate_fishbone_diagram | 生成鱼骨图 |
| generate_flow_diagram | 生成流程图 |
| generate_network_graph | 生成关系网络图 |
| generate_organization_chart | 生成组织架构图 |
| generate_district_map | 生成区域分布地图（中国） |
| generate_path_map | 生成路线地图（旅游路线） |
| generate_pin_map | 生成点标注地图（POI分布） |
| generate_liquid_chart | 生成水波图，展示百分比 |
| generate_dual_axes_chart | 生成双轴图表 |
| generate_word_cloud_chart | 生成词云图 |
| generate_venn_chart | 生成韦恩图 |

---

## 3. bmi-mcp（BMI体重指数）

**功能**：根据身高体重计算BMI指数，提供健康评估与建议。

**工具列表**（共 1 个）：

| 工具名 | 功能 |
|--------|------|
| BMI体重指数 | 根据身高、体重参数查询BMI指数，返回健康评估与建议 |

---

## 4. bw-ir（发票验证）

**功能**：验证增值税发票，普通发票，电子发票等14类票据的真伪。

**工具列表**（共 1 个）：

| 工具名 | 功能 |
|--------|------|
| invoice_verification | 验证发票真实性和合规性，支持多种发票类型核验 |

---

## 5. didi（滴滴出行）

**功能**：打车、路线规划、订单管理、司机位置追踪。

**工具列表**（共 13 个）：

| 工具名 | 功能 |
|--------|------|
| taxi_estimate | 查看网约车可用车型及预估价格 |
| taxi_create_order | 创建打车订单 |
| taxi_query_order | 查询订单状态、司机信息、预估到达时间 |
| taxi_cancel_order | 取消打车订单 |
| taxi_get_driver_location | 获取司机实时位置 |
| taxi_generate_ride_app_link | 生成跳转App/小程序的深度链接 |
| maps_direction_driving | 驾车路径规划 |
| maps_direction_transit | 公交+地铁综合通勤方案 |
| maps_direction_bicycling | 骑行路径规划 |
| maps_direction_walking | 步行路线规划 |
| maps_textsearch | 关键词搜索POI地点 |
| maps_place_around | 周边地点搜索 |
| maps_regeocode | 经纬度转地址信息 |

---

## 6. food-detective（美食推荐）

**功能**：根据地名推荐当地特色美食。

**工具列表**（共 1 个）：

| 工具名 | 功能 |
|--------|------|
| 推荐美食 | 传入地名，返回5条当地美食和推荐理由 |

---

## 7. how-to-cook（菜谱大全）

**功能**：中餐菜谱查询、分类浏览、智能膳食推荐。

**工具列表**（共 5 个）：

| 工具名 | 功能 |
|--------|------|
| mcp_howtocook_getAllRecipes | 获取所有菜谱 |
| mcp_howtocook_getRecipesByCategory | 按分类查询（水产/早餐/荤菜/素菜/汤/主食等） |
| mcp_howtocook_getRecipeById | 查询指定菜谱详情，含食材与步骤 |
| mcp_howtocook_whatToEat | 根据人数推荐菜品组合 |
| mcp_howtocook_recommendMeals | 根据忌口/过敏原智能推荐一周膳食计划 |

---

## 8. market-cmapi（区域新闻）

**功能**：中国各省市区域新闻查询。

**工具列表**（共 2 个）：

| 工具名 | 功能 |
|--------|------|
| 查询地区新闻 | 中国各省市区域新闻查询 |
| 查询支持的新闻地区 | 查询该API支持的省市列表 |

---

## 9. openscad（3D建模）

**功能**：通过自然语言描述生成3D模型，支持导出STL等格式。

**工具列表**（共 7 个）：

| 工具名 | 功能 |
|--------|------|
| create_3d_model | 从自然语言描述创建3D模型 |
| modify_3d_model | 修改现有3D模型 |
| export_model | 导出3D模型为指定格式（STL等） |
| list_models | 列出所有已生成的模型 |
| get_supported_3d_shapes | 获取支持的3D形状类型 |
| generate_image | 用Venice.ai生成图片 |
| generate_image_gemini | 用Google Gemini生成图片 |

---

## 10. vision-mcp（视觉理解）

**功能**：分析图片内容，提供详细文字描述。

**工具列表**（共 1 个）：

| 工具名 | 功能 |
|--------|------|
| analyze_image | 分析图片内容并提供详细描述 |

---

## 11. gezhe（PPT生成）

**功能**：通过主题词生成PPT演示文稿。

**工具列表**（共 1 个）：

| 工具名 | 功能 |
|--------|------|
| generate_ppt_by_topic | 根据主题生成PowerPoint演示文稿 |

---

## 12. playwright（浏览器自动化）

**功能**：自动化控制浏览器，支持网页浏览、截图、表单填写。

**工具列表**（共 8 个）：

| 工具名 | 功能 |
|--------|------|
| navigate | 导航到指定URL |
| screenshot | 截取当前页面并保存到文件 |
| get_page_content | 获取完整HTML内容 |
| get_text | 获取页面元素文本 |
| click | 点击页面元素 |
| fill | 填写表单输入框 |
| wait_for_selector | 等待元素出现 |
| close_browser | 关闭浏览器 |

---

## 13. pandoc（文档格式转换）

**功能**：支持Markdown、HTML、DOCX、PDF、LaTeX等格式互相转换。

**工具列表**（共 1 个）：

| 工具名 | 功能 |
|--------|------|
| convert-contents | 在不同文档格式间转换（Markdown/HTML/DOCX/PDF/LaTeX等） |

---

## 14. doc-forge（文档处理）

**功能**：PDF分割/合并、文档读取、格式转换、文本处理。

**工具列表**（共 16 个）：

| 工具名 | 功能 |
|--------|------|
| document_reader | 读取PDF/DOCX/TXT/HTML/CSV文档内容 |
| pdf_merger | 合并多个PDF文件 |
| pdf_splitter | 分割PDF文件 |
| docx_to_pdf | DOCX转PDF |
| docx_to_html | DOCX转HTML（保留格式） |
| html_cleaner | 清理HTML冗余标签 |
| html_to_text | HTML转纯文本 |
| html_to_markdown | HTML转Markdown |
| html_extract_resources | 提取HTML中的图片/视频/链接资源 |
| html_formatter | 格式化美化HTML代码 |
| text_diff | 对比两个文本文件差异 |
| text_splitter | 按分隔符或行数分割文本 |
| text_formatter | 格式化文本（缩进/行距） |
| text_encoding_converter | 文本编码转换（UTF-8/GBK/Big5等） |
| excel_read | 读取Excel文件并转为JSON |
| format_convert | Markdown/HTML/XML/JSON格式互转 |

---

## 15. excel（Excel操作）

**功能**：读取、写入、格式化Excel表格，创建表格。

**工具列表**（共 6 个）：

| 工具名 | 功能 |
|--------|------|
| excel_read_sheet | 分页读取Excel表格数据 |
| excel_write_to_sheet | 向Excel写入数据 |
| excel_format_range | 格式化单元格（字体/背景/边框/数字格式） |
| excel_create_table | 在工作表中创建表格 |
| excel_copy_sheet | 复制工作表 |
| excel_describe_sheets | 获取所有Sheet信息 |

---

## 16. minimax（MiniMax多媒体）

**功能**：图片生成、视频生成，音乐生成、语音合成、声音克隆。

**工具列表**（共 9 个）：

| 工具名 | 功能 |
|--------|------|
| text_to_image | 文本生成图片 |
| generate_video | 文本/图片生成视频 |
| music_generation | 根据歌词和风格生成音乐 |
| text_to_audio | 文本转语音，支持多种音色 |
| play_audio | 播放音频文件（WAV/MP3） |
| list_voices | 列出所有可用音色 |
| voice_clone | 克隆声音 |
| voice_design | 根据描述生成新音色 |
| query_video_generation | 查询视频生成任务状态 |

---

## 17. qrcode-mcp（二维码）

**功能**：生成二维码图片。

**工具列表**（共 1 个）：

| 工具名 | 功能 |
|--------|------|
| 二维码生成 | 将文本/URL生成二维码图片 |

---

## 18. stock-quote（行情报价）

**功能**：A股/港股/美股/期货/外汇实时行情与K线数据。

**工具列表**（共 21 个）：

| 工具名 | 功能 |
|--------|------|
| A股报价 | A股实时行情报价 |
| A股排行 | A股涨跌幅/成交量等排行 |
| A股K线 | A股K线数据（1分钟/5分钟/日K/月K等） |
| A股K线复权 | A股复权K线数据 |
| 港股报价 | 港股实时行情 |
| 港股排行 | 港股排行榜 |
| 港股K线 | 港股K线数据 |
| 美股报价 | 美股实时报价 |
| 美股排行 | 美股排行榜 |
| 美股K线 | 美股K线数据 |
| 美股品种 | 美股品种查询 |
| 内盘期货报价 | 国内期货实时报价 |
| 内盘期货合约 | 国内期货合约查询 |
| 内盘期货K线 | 国内期货K线 |
| 外盘期货报价 | 国外期货报价 |
| 外盘期货合约 | 国外期货合约 |
| 外盘期货K线 | 国外期货K线 |
| 外汇报价 | 外汇实时汇率 |
| 外汇K线 | 外汇K线 |
| 全球指数报价 | 全球指数行情 |
| 全球指数K线 | 全球指数K线 |

---

## 19. amap（高德地图）

**功能**：地理编码、路径规划、天气查询、POI搜索。

**工具列表**（共 12 个）：

| 工具名 | 功能 |
|--------|------|
| maps_geo | 地址转经纬度（地理编码） |
| maps_regeocode | 经纬度转地址（逆地理编码） |
| maps_ip_location | IP地址定位 |
| maps_weather | 按城市查询天气 |
| maps_text_search | 关键词搜索POI |
| maps_around_search | 周边地点搜索 |
| maps_search_detail | 查询POI详细信息 |
| maps_direction_driving | 驾车路径规划 |
| maps_direction_transit_integrated | 公交综合路线规划 |
| maps_direction_walking | 步行路线规划 |
| maps_bicycling | 骑行路线规划 |
| maps_distance | 测量两点间距离 |

---

## 20. github（GitHub操作）

**功能**：仓库管理、Issue/PR操作、代码搜索、代码评审。

**工具列表**（共 26 个）：

| 工具名 | 功能 |
|--------|------|
| create_repository | 创建新仓库 |
| fork_repository | Fork仓库 |
| get_file_contents | 获取文件/目录内容 |
| push_files | 批量推送文件到仓库 |
| create_or_update_file | 创建或更新单个文件 |
| create_branch | 创建分支 |
| list_commits | 获取提交历史 |
| create_issue | 创建Issue |
| update_issue | 更新Issue状态/标签 |
| get_issue | 获取Issue详情 |
| add_issue_comment | 添加Issue评论 |
| list_issues | 列出Issue列表 |
| create_pull_request | 创建Pull Request |
| get_pull_request | 获取PR详情 |
| list_pull_requests | 列出PR列表 |
| create_pull_request_review | 创建PR评审 |
| get_pull_request_reviews | 获取PR评审列表 |
| get_pull_request_files | 获取PR变更文件列表 |
| get_pull_request_comments | 获取PR评论 |
| get_pull_request_status | 获取PR CI状态 |
| merge_pull_request | 合并PR |
| update_pull_request_branch | 更新PR分支 |
| search_repositories | 搜索仓库 |
| search_code | 搜索代码 |
| search_issues | 搜索Issue和PR |
| search_users | 搜索GitHub用户 |

---

## 21. sqlite（SQLite数据库）

**功能**：本地SQLite数据库的CRUD操作。

**工具列表**（共 5 个）：

| 工具名 | 功能 |
|--------|------|
| list_tables | 列出所有表 |
| describe_table | 获取表结构 |
| read_query | 执行SELECT查询 |
| write_query | 执行INSERT/UPDATE/DELETE |
| create_table | 创建新表 |

---

## 22. weather（天气预报）

**功能**：当前天气、天气预报、空气质量查询。

**工具列表**（共 3 个）：

| 工具名 | 功能 |
|--------|------|
| get_weather | 获取当前天气 |
| get_forecast | 获取3-5天天气预报 |
| get_air_quality | 获取空气质量（AQI/PM2.5等） |

---

## 23. local_time（本地时间）

**功能**：获取当前本地时间。

**工具列表**（共 1 个）：

| 工具名 | 功能 |
|--------|------|
| get_current_time | 获取当前本地时间 |

---

## ❌ 连接失败 / 已禁用的MCP

| MCP名称 | 状态 | 说明 |
|---------|------|------|
| luckin | 已禁用 | 瑞幸咖啡（已禁用） |
| mbti | 已禁用 | MBTI性格测试（已禁用） |
| gf-windmill | 已禁用 | 广发WindMill（已禁用） |
| mmb-mcp | 连接失败(401) | 慢慢买MCP（认证失败） |
| xhs-toolkit | 连接超时 | 小红书工具包（连接超时） |
| xhs-toolkit-http | 连接失败 | 小红书HTTP服务（本地服务未启动） |

---

*文档由 Hermes Agent 自动生成，如有问题请联系维护者。*
