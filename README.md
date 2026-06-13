# 旺旺Agent - API工具文档

> 记录所有可用的MCP（Model Context Protocol）接口

## 更新日期
2026-06-13

---

## 📍 地图与出行

### 高德地图 (amap) — 12工具
| 工具 | 功能 |
|------|------|
| maps_geo | 地址转换为经纬度坐标 |
| maps_regeocode | 经纬度坐标转换为行政区划地址 |
| maps_ip_location | IP地址定位 |
| maps_weather | 城市天气预报 |
| maps_search_detail | 查询POI详细信息 |
| maps_bicycling | 骑行路线规划 |
| maps_direction_walking | 步行路线规划 |
| maps_direction_driving | 驾车路线规划 |
| maps_direction_transit_integrated | 公交综合路线规划 |
| maps_distance | 两点间距离测量 |
| maps_text_search | 关键词搜索POI地点 |
| maps_around_search | 周边地点搜索 |

### 滴滴出行 (didi) — 13工具
| 工具 | 功能 |
|------|------|
| maps_textsearch | 地点关键词搜索 |
| maps_regeocode | 坐标转地址 |
| maps_place_around | 周边POI搜索 |
| maps_direction_driving | 驾车路线 |
| maps_direction_transit | 公交路线 |
| maps_direction_walking | 步行路线 |
| maps_direction_bicycling | 骑行路线 |
| taxi_estimate | 预估打车价格 |
| taxi_create_order | 创建打车订单 |
| taxi_query_order | 查询订单状态 |
| taxi_cancel_order | 取消打车订单 |
| taxi_get_driver_location | 实时司机位置 |
| taxi_generate_ride_app_link | 生成打车App深度链接 |

---

## 📊 金融数据

### 股票行情 (stock-quote) — 21工具
| 工具 | 功能 |
|------|------|
| A股报价 | 沪深京A股实时报价 |
| A股K线 | A股K线数据（1分钟/日/周/月） |
| A股K线复权 | A股复权K线数据 |
| A股排行 | A股涨跌幅/成交额排行 |
| 港股报价 | 港股实时报价 |
| 港股K线 | 港股K线数据 |
| 港股排行 | 港股成交排行 |
| 美股报价 | 美股实时报价 |
| 美股K线 | 美股K线数据 |
| 美股排行 | 美股涨跌幅排行 |
| 美股品种 | 美股交易品种 |
| 外汇报价 | 外汇实时报价 |
| 外汇K线 | 外汇K线数据 |
| 全球指数报价 | 全球主要指数实时报价 |
| 全球指数K线 | 全球指数K线 |
| 内盘期货报价 | 国内期货实时报价 |
| 内盘期货K线 | 国内期货K线 |
| 内盘期货合约 | 国内期货合约信息 |
| 外盘期货报价 | 外盘期货实时报价 |
| 外盘期货K线 | 外盘期货K线 |
| 外盘期货合约 | 外盘期货合约信息 |

### 金融图表 (antv-chart) — 124工具
股票：公司信息、行情（复权/未复权）、除权因子、利润表、资产负债表、现金流量表、业绩快报、重大合同、高管持股、股权质押、股权冻结、股份回购、配股、增发、要约收购、吸收合并、特别处理、股东户数、机构持仓、关联交易、管理层、曾用名、融资融券、定期报告、分红。

基金：基本信息、净值历史、复权净值、回报率、持仓（股票/债券/基金/行业）、资产配置、持有人结构、申购赎回状态、分红、拆分折算、费率、投资标的、业绩基准、关联基金、奖项、经理信息、三级分类。

指数：基本信息、历史行情、成分股、业绩比较基准。

ETF：持仓清单、申购赎回清单。

宏观：CPI、PPI、货币供应量、社融存量、国债收益率、交易日历。

| 工具前缀 | 功能 |
|------|------|
| list_stock_* | 股票相关数据查询 |
| list_fund_* | 基金相关数据查询 |
| list_index_* | 指数相关数据查询 |
| get_* | 单一实体信息查询 |
| search | 金融产品关键字搜索 |
| generate_chart / generate_nex_chart | ECharts图表生成 |
| list_economic_cn_* | CPI/PPI查询 |
| list_money_* | 货币/国债数据查询 |
| list_gover_bond_yield | 国债收益率曲线 |
| list_social_financing_sto | 社会融资规模 |

### 图表生成 (antv-visual) — 25工具
| 工具 | 功能 |
|------|------|
| generate_line_chart | 折线图（趋势） |
| generate_column_chart | 柱状图（对比） |
| generate_bar_chart | 条形图（横向对比） |
| generate_pie_chart | 饼图（占比） |
| generate_area_chart | 面积图 |
| generate_scatter_chart | 散点图（关联） |
| generate_histogram_chart | 直方图（分布） |
| generate_boxplot_chart | 箱线图（统计） |
| generate_violin_chart | 小提琴图 |
| generate_radar_chart | 雷达图（多维） |
| generate_sankey_chart | 桑基图（流向） |
| generate_funnel_chart | 漏斗图（转化） |
| generate_treemap_chart | 矩形树图 |
| generate_network_graph | 网络图 |
| generate_mind_map | 思维导图 |
| generate_organization_chart | 组织架构图 |
| generate_flow_diagram | 流程图 |
| generate_fishbone_diagram | 鱼骨图 |
| generate_venn_chart | 韦恩图 |
| generate_word_cloud_chart | 词云图 |
| generate_liquid_chart | 水球图 |
| generate_dual_axes_chart | 双轴图 |
| generate_district_map | 区域地图（中国） |
| generate_path_map | 路线地图 |
| generate_pin_map | 点位地图 |

---

## 🎨 AI生成

### MiniMax (minimax) — 9工具
| 工具 | 功能 |
|------|------|
| text_to_image | 图片生成 |
| generate_video | 视频生成 |
| text_to_audio | 语音合成（TTS） |
| music_generation | 音乐生成 |
| voice_clone | 声音克隆 |
| voice_design | 语音风格设计 |
| list_voices | 音色列表 |
| play_audio | 播放音频 |
| query_video_generation | 视频生成状态 |

### OpenSCAD (openscad) — 7工具
| 工具 | 功能 |
|------|------|
| create_3d_model | 自然语言生成3D模型 |
| modify_3d_model | 修改已有3D模型 |
| export_model | 导出STL等格式 |
| list_models | 列出已生成模型 |
| generate_image | Venice.ai图片生成 |
| generate_image_gemini | Gemini图片生成 |
| get_supported_3d_shapes | 支持的几何体列表 |

### 智谱视觉 (vision-mcp) — 1工具
| 工具 | 功能 |
|------|------|
| analyze_image | 图片内容理解与描述 |

### 二维码 (qrcode-mcp) — 1工具
| 工具 | 功能 |
|------|------|
| 二维码生成 | 生成二维码图片 |

---

## 📄 文档处理

### 文档工厂 (doc-forge) — 16工具
| 工具 | 功能 |
|------|------|
| document_reader | 读取PDF/DOCX/TXT/HTML/CSV |
| pdf_merger | 合并多个PDF |
| pdf_splitter | 拆分PDF |
| docx_to_pdf | Word转PDF |
| docx_to_html | Word转HTML |
| html_to_text | HTML转纯文本 |
| html_to_markdown | HTML转Markdown |
| html_cleaner | 清理HTML冗余标签 |
| html_formatter | 格式化HTML |
| html_extract_resources | 提取HTML资源 |
| text_diff | 对比两个文本文件差异 |
| text_splitter | 按分隔符/行数拆分文本 |
| text_formatter | 格式化文本 |
| text_encoding_converter | 文本编码转换 |
| excel_read | 读取Excel文件 |
| format_convert | 文档格式互转 |

### Excel (excel) — 6工具
| 工具 | 功能 |
|------|------|
| excel_read_sheet | 读取工作表数据 |
| excel_write_to_sheet | 写入工作表数据 |
| excel_format_range | 格式化单元格 |
| excel_describe_sheets | 列出工作表信息 |
| excel_create_table | 创建Excel表格 |
| excel_copy_sheet | 复制工作表 |

### Pandoc (pandoc) — 1工具
| 工具 | 功能 |
|------|------|
| convert-contents | 文档格式转换（Markdown↔HTML↔PDF↔DOCX等） |

---

## 🌐 浏览器与自动化

### Playwright (playwright) — 8工具
| 工具 | 功能 |
|------|------|
| navigate | 打开指定URL |
| screenshot | 页面截图 |
| get_page_content | 获取页面HTML |
| get_text | 获取元素文本 |
| click | 点击页面元素 |
| fill | 填写表单字段 |
| wait_for_selector | 等待元素出现 |
| close_browser | 关闭浏览器 |

---

## 🛠️ 数据库与开发

### SQLite (sqlite) — 5工具
| 工具 | 功能 |
|------|------|
| read_query | 执行SELECT查询 |
| write_query | 执行INSERT/UPDATE/DELETE |
| create_table | 创建数据表 |
| list_tables | 列出所有表 |
| describe_table | 查看表结构 |

### GitHub (github) — 26工具
| 工具 | 功能 |
|------|------|
| search_repositories | 搜索仓库 |
| search_code | 搜索代码 |
| search_issues | 搜索Issue/PR |
| search_users | 搜索用户 |
| get_file_contents | 获取文件内容 |
| create_repository | 创建仓库 |
| fork_repository | Fork仓库 |
| push_files | 推送多个文件 |
| create_or_update_file | 创建/更新单文件 |
| create_branch | 创建分支 |
| list_commits | 查看提交记录 |
| create_issue | 创建Issue |
| get_issue | 查看Issue详情 |
| list_issues | 列出Issue |
| update_issue | 更新Issue |
| add_issue_comment | 评论Issue |
| create_pull_request | 创建PR |
| get_pull_request | 查看PR详情 |
| list_pull_requests | 列出PR |
| create_pull_request_review | 提交PR Review |
| merge_pull_request | 合并PR |
| get_pull_request_files | 查看PR改动文件 |
| get_pull_request_status | 查看CI状态 |
| get_pull_request_comments | 查看PR评论 |
| get_pull_request_reviews | 查看PR Reviews |
| update_pull_request_branch | 更新PR分支 |

---

## 🍳 生活服务

### 美食 (food-detective) — 1工具
| 工具 | 功能 |
|------|------|
| 推荐美食 | 传入地名返回5条当地美食推荐 |

### 菜谱 (how-to-cook) — 5工具
| 工具 | 功能 |
|------|------|
| mcp_howtocook_whatToEat | 随机推荐菜品 |
| mcp_howtocook_recommendMeals | 智能推荐一周食谱 |
| mcp_howtocook_getRecipesByCategory | 按分类查菜谱 |
| mcp_howtocook_getRecipeById | 查询菜谱详情 |
| mcp_howtocook_getAllRecipes | 获取所有菜谱 |

### 健康 (bmi-mcp) — 1工具
| 工具 | 功能 |
|------|------|
| BMI体重指数 | 根据身高体重计算BMI并给出健康建议 |

---

## 🗓️ 工具类

### 天气 (weather) — 3工具
| 工具 | 功能 |
|------|------|
| get-forecast | 指定坐标天气预报 |
| get-alerts | 天气预警 |
| enable-air-quality | 空气质量查询 |

### 时间 (local_time) — 1工具
| 工具 | 功能 |
|------|------|
| get_current_time | 获取当前本地时间 |

### 发票 (bw-ir) — 1工具
| 工具 | 功能 |
|------|------|
| invoice_verification | 验证发票真实性与合规性 |

### 新闻 (market-cmapi) — 2工具
| 工具 | 功能 |
|------|------|
| 查询地区新闻 | 查询指定地区新闻 |
| 查询支持的新闻地区 | 查看支持的地区列表 |

### PPT (gezhe) — 1工具
| 工具 | 功能 |
|------|------|
| generate_ppt_by_topic | 根据主题生成PPT |

---

## 📋 MCP总览

| MCP名称 | 状态 | 工具数 |
|---------|------|--------|
| antv-chart | ✅ 已启用 | 124 |
| github | ✅ 已启用 | 26 |
| antv-visual | ✅ 已启用 | 25 |
| stock-quote | ✅ 已启用 | 21 |
| doc-forge | ✅ 已启用 | 16 |
| didi | ✅ 已启用 | 13 |
| amap | ✅ 已启用 | 12 |
| minimax | ✅ 已启用 | 9 |
| playwright | ✅ 已启用 | 8 |
| openscad | ✅ 已启用 | 7 |
| excel | ✅ 已启用 | 6 |
| how-to-cook | ✅ 已启用 | 5 |
| sqlite | ✅ 已启用 | 5 |
| weather | ✅ 已启用 | 3 |
| market-cmapi | ✅ 已启用 | 2 |
| bmi-mcp | ✅ 已启用 | 1 |
| bw-ir | ✅ 已启用 | 1 |
| food-detective | ✅ 已启用 | 1 |
| qrcode-mcp | ✅ 已启用 | 1 |
| vision-mcp | ✅ 已启用 | 1 |
| gezhe | ✅ 已启用 | 1 |
| pandoc | ✅ 已启用 | 1 |
| local_time | ✅ 已启用 | 1 |
| luckin | ⛔ 已禁用 | — |
| mbti | ⛔ 已禁用 | — |
| gf-windmill | ⛔ 已禁用 | — |
| mmb-mcp | ⛔ 连接失败 | — |

**总计：24个MCP已启用，3个已禁用，1个连接失败，共约270个工具**

---

*本文档由旺旺Agent自动生成，更新于 2026-06-13*
