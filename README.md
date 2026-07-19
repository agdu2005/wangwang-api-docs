# WangWang API 文档

> 更新日期: 2026-07-19 | 数据来源: Hermes Agent MCP 健康检查日志

## 概览

- **MCP 服务器总数**: 23
- **工具总数**: 306
- **注意**: 以下数据来自最近一次完整启动日志（2026-06-26），当前 gateway MCP 配置可能需要重新启用

---

## 🔌 amap

- **传输方式**: stdio
- **工具数量**: 12

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_amap_maps_regeocode` | Maps Regeocode |
| `mcp_amap_maps_geo` | Maps Geo |
| `mcp_amap_maps_ip_location` | Maps Ip Location |
| `mcp_amap_maps_weather` | Maps Weather |
| `mcp_amap_maps_search_detail` | Maps Search Detail |
| `mcp_amap_maps_bicycling` | Maps Bicycling |
| `mcp_amap_maps_direction_walking` | Maps Direction Walking |
| `mcp_amap_maps_direction_driving` | Maps Direction Driving |
| `mcp_amap_maps_direction_transit_integrated` | Maps Direction Transit Integrated |
| `mcp_amap_maps_distance` | Maps Distance |
| `mcp_amap_maps_text_search` | Maps Text Search |
| `mcp_amap_maps_around_search` | Maps Around Search |

## 🌐 antv-chart

- **传输方式**: HTTP
- **工具数量**: 128

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_antv_chart_list_stocks_public_offering_place` | Mcp Antv Chart List Stocks Public Offering Place |
| `mcp_antv_chart_list_stocks_dividends` | Mcp Antv Chart List Stocks Dividends |
| `mcp_antv_chart_list_stock_offerings` | Mcp Antv Chart List Stock Offerings |
| `mcp_antv_chart_list_stocks_rights_issue_res` | Mcp Antv Chart List Stocks Rights Issue Res |
| `mcp_antv_chart_list_stock_top10_circulating_shareh` | Mcp Antv Chart List Stock Top10 Circulating Shareh |
| `mcp_antv_chart_list_stock_capital_changes` | Mcp Antv Chart List Stock Capital Changes |
| `mcp_antv_chart_list_stock_freeze_details` | Mcp Antv Chart List Stock Freeze Details |
| `mcp_antv_chart_list_stock_pledge_details` | Mcp Antv Chart List Stock Pledge Details |
| `mcp_antv_chart_list_stock_repurchase_plans` | Mcp Antv Chart List Stock Repurchase Plans |
| `mcp_antv_chart_list_stock_institutional_holdings_stats` | Mcp Antv Chart List Stock Institutional Holdings Stats |
| `mcp_antv_chart_list_stock_tender_offers` | Mcp Antv Chart List Stock Tender Offers |
| `mcp_antv_chart_get_trade_special_date` | Mcp Antv Chart Get Trade Special Date |
| `mcp_antv_chart_list_stk_income_state_pit` | Mcp Antv Chart List Stk Income State Pit |
| `mcp_antv_chart_list_stk_balan_sheet_pit` | Mcp Antv Chart List Stk Balan Sheet Pit |
| `mcp_antv_chart_list_stock_cash_flows_pit` | Mcp Antv Chart List Stock Cash Flows Pit |
| `mcp_antv_chart_list_fund_all` | Mcp Antv Chart List Fund All |
| `mcp_antv_chart_list_stock_all` | Mcp Antv Chart List Stock All |
| `mcp_antv_chart_list_fund_hold_industry` | Mcp Antv Chart List Fund Hold Industry |
| `mcp_antv_chart_list_index_quote_barch` | Mcp Antv Chart List Index Quote Barch |
| `mcp_antv_chart_list_report_institutions` | Mcp Antv Chart List Report Institutions |
| `mcp_antv_chart_list_stock_unadjusted_quotes` | Mcp Antv Chart List Stock Unadjusted Quotes |
| `mcp_antv_chart_list_stock_share_adj_factors` | Mcp Antv Chart List Stock Share Adj Factors |
| `mcp_antv_chart_get_company_profiles` | Mcp Antv Chart Get Company Profiles |
| `mcp_antv_chart_list_index_quotes` | Mcp Antv Chart List Index Quotes |
| `mcp_antv_chart_list_stock_report_schema` | Mcp Antv Chart List Stock Report Schema |
| `mcp_antv_chart_list_stock_major_contracts` | Mcp Antv Chart List Stock Major Contracts |
| `mcp_antv_chart_get_stock_margin_securities` | Mcp Antv Chart Get Stock Margin Securities |
| `mcp_antv_chart_list_stock_executive_shareholding_change` | Mcp Antv Chart List Stock Executive Shareholding Change |
| `mcp_antv_chart_get_cn_trade_calender_list` | Mcp Antv Chart Get Cn Trade Calender List |
| `mcp_antv_chart_list_stock_management_dirs` | Mcp Antv Chart List Stock Management Dirs |
| `mcp_antv_chart_list_stock_core_mgmt_changes` | Mcp Antv Chart List Stock Core Mgmt Changes |
| `mcp_antv_chart_list_stock_related_transactions` | Mcp Antv Chart List Stock Related Transactions |
| `mcp_antv_chart_list_industries` | Mcp Antv Chart List Industries |
| `mcp_antv_chart_get_stock_rights_issues` | Mcp Antv Chart Get Stock Rights Issues |
| `mcp_antv_chart_list_concepts` | Mcp Antv Chart List Concepts |
| `mcp_antv_chart_list_stocks_dividends` | Mcp Antv Chart List Stocks Dividends |
| `mcp_antv_chart_list_stocks_public_offering_place` | Mcp Antv Chart List Stocks Public Offering Place |
| `mcp_antv_chart_get_stock_basic_info` | Mcp Antv Chart Get Stock Basic Info |
| `mcp_antv_chart_list_stocks_rights_issue_res` | Mcp Antv Chart List Stocks Rights Issue Res |
| `mcp_antv_chart_list_stock_offerings` | Mcp Antv Chart List Stock Offerings |
| `mcp_antv_chart_list_stock_capital_changes` | Mcp Antv Chart List Stock Capital Changes |
| `mcp_antv_chart_list_stock_top10_circulating_shareh` | Mcp Antv Chart List Stock Top10 Circulating Shareh |
| `mcp_antv_chart_list_stock_pledge_details` | Mcp Antv Chart List Stock Pledge Details |
| `mcp_antv_chart_list_stock_freeze_details` | Mcp Antv Chart List Stock Freeze Details |
| `mcp_antv_chart_list_stock_absorption_mergers` | Mcp Antv Chart List Stock Absorption Mergers |
| `mcp_antv_chart_list_stock_repurchase_plans` | Mcp Antv Chart List Stock Repurchase Plans |
| `mcp_antv_chart_list_stock_tender_offers` | Mcp Antv Chart List Stock Tender Offers |
| `mcp_antv_chart_list_stock_earnings_bulletins` | Mcp Antv Chart List Stock Earnings Bulletins |
| `mcp_antv_chart_list_stock_cash_flows` | Mcp Antv Chart List Stock Cash Flows |
| `mcp_antv_chart_list_stock_income_statements` | Mcp Antv Chart List Stock Income Statements |
| `mcp_antv_chart_list_stock_balance_sheet` | Mcp Antv Chart List Stock Balance Sheet |
| `mcp_antv_chart_list_stock_adjusted_quotes` | Mcp Antv Chart List Stock Adjusted Quotes |
| `mcp_antv_chart_list_fund_daily_quotes` | Mcp Antv Chart List Fund Daily Quotes |
| `mcp_antv_chart_list_stock_special_notices` | Mcp Antv Chart List Stock Special Notices |
| `mcp_antv_chart_list_fund_adj_quotes` | Mcp Antv Chart List Fund Adj Quotes |
| `mcp_antv_chart_get_fund_code_assoc` | Mcp Antv Chart Get Fund Code Assoc |
| `mcp_antv_chart_get_fund_basic_info` | Mcp Antv Chart Get Fund Basic Info |
| `mcp_antv_chart_get_fund_listings_record` | Mcp Antv Chart Get Fund Listings Record |
| `mcp_antv_chart_get_fund_categories` | Mcp Antv Chart Get Fund Categories |
| `mcp_antv_chart_get_fund_manager_basic_info` | Mcp Antv Chart Get Fund Manager Basic Info |
| `mcp_antv_chart_list_stock_holder_cnt` | Mcp Antv Chart List Stock Holder Cnt |
| `mcp_antv_chart_list_subscription_redemption_status` | Mcp Antv Chart List Subscription Redemption Status |
| `mcp_antv_chart_list_fund_invest_targets` | Mcp Antv Chart List Fund Invest Targets |
| `mcp_antv_chart_get_stock_former_names` | Mcp Antv Chart Get Stock Former Names |
| `mcp_antv_chart_list_fund_perf_benchmarks` | Mcp Antv Chart List Fund Perf Benchmarks |
| `mcp_antv_chart_list_fund_fee_structures` | Mcp Antv Chart List Fund Fee Structures |
| `mcp_antv_chart_list_stock_institutional_holdings_stats` | Mcp Antv Chart List Stock Institutional Holdings Stats |
| `mcp_antv_chart_get_fund_award_records` | Mcp Antv Chart Get Fund Award Records |
| `mcp_antv_chart_get_stock_industries` | Mcp Antv Chart Get Stock Industries |
| `mcp_antv_chart_list_fund_nav_history` | Mcp Antv Chart List Fund Nav History |
| `mcp_antv_chart_list_currency_yield_history` | Mcp Antv Chart List Currency Yield History |
| `mcp_antv_chart_list_fund_adj_navs` | Mcp Antv Chart List Fund Adj Navs |
| `mcp_antv_chart_list_fund_return_rate` | Mcp Antv Chart List Fund Return Rate |
| `mcp_antv_chart_list_perf_benchmark_quote` | Mcp Antv Chart List Perf Benchmark Quote |
| `mcp_antv_chart_list_fund_share_splits` | Mcp Antv Chart List Fund Share Splits |
| `mcp_antv_chart_list_fund_dividend_distributions` | Mcp Antv Chart List Fund Dividend Distributions |
| `mcp_antv_chart_list_hk_stock_dividends` | Mcp Antv Chart List Hk Stock Dividends |
| `mcp_antv_chart_list_fund_portfolio_asset_holdings` | Mcp Antv Chart List Fund Portfolio Asset Holdings |
| `mcp_antv_chart_list_fund_portfolio_stock_holdings` | Mcp Antv Chart List Fund Portfolio Stock Holdings |
| `mcp_antv_chart_generate_chart` | Mcp Antv Chart Generate Chart |
| `mcp_antv_chart_list_fund_portfolio_bond_holdings` | Mcp Antv Chart List Fund Portfolio Bond Holdings |
| `mcp_antv_chart_generate_nex_chart` | Mcp Antv Chart Generate Nex Chart |
| `mcp_antv_chart_list_portfolio_fund_holdings` | Mcp Antv Chart List Portfolio Fund Holdings |
| `mcp_antv_chart_list_fund_shares` | Mcp Antv Chart List Fund Shares |
| `mcp_antv_chart_list_fund_hold_structures` | Mcp Antv Chart List Fund Hold Structures |
| `mcp_antv_chart_list_etf_constituent_stks` | Mcp Antv Chart List Etf Constituent Stks |
| `mcp_antv_chart_list_etf_sub_red_lists` | Mcp Antv Chart List Etf Sub Red Lists |
| `mcp_antv_chart_list_fund_fin_inds_q` | Mcp Antv Chart List Fund Fin Inds Q |
| `mcp_antv_chart_list_fund_fin_inds` | Mcp Antv Chart List Fund Fin Inds |
| `mcp_antv_chart_list_economic_cn_cpi` | Mcp Antv Chart List Economic Cn Cpi |
| `mcp_antv_chart_list_economic_cn_ppi` | Mcp Antv Chart List Economic Cn Ppi |
| `mcp_antv_chart_list_industry_hold_fund` | Mcp Antv Chart List Industry Hold Fund |
| `mcp_antv_chart_list_concept_hold_fund` | Mcp Antv Chart List Concept Hold Fund |
| `mcp_antv_chart_is_trade_date` | Mcp Antv Chart Is Trade Date |
| `mcp_antv_chart_get_index_basic_info` | Mcp Antv Chart Get Index Basic Info |
| `mcp_antv_chart_search` | Mcp Antv Chart Search |
| `mcp_antv_chart_list_fund_all` | Mcp Antv Chart List Fund All |
| `mcp_antv_chart_list_stock_all` | Mcp Antv Chart List Stock All |
| `mcp_antv_chart_list_money_supplies` | Mcp Antv Chart List Money Supplies |
| `mcp_antv_chart_list_gover_bond_yield` | Mcp Antv Chart List Gover Bond Yield |
| `mcp_antv_chart_list_money_market_repo_in` | Mcp Antv Chart List Money Market Repo In |
| `mcp_antv_chart_list_social_financing_sto` | Mcp Antv Chart List Social Financing Sto |
| `mcp_antv_chart_list_stock_absorption_mergers` | Mcp Antv Chart List Stock Absorption Mergers |
| `mcp_antv_chart_list_stock_special_notices` | Mcp Antv Chart List Stock Special Notices |
| `mcp_antv_chart_get_stock_basic_info` | Mcp Antv Chart Get Stock Basic Info |
| `mcp_antv_chart_list_stock_unadjusted_quotes` | Mcp Antv Chart List Stock Unadjusted Quotes |
| `mcp_antv_chart_get_stock_former_names` | Mcp Antv Chart Get Stock Former Names |
| `mcp_antv_chart_list_stock_adjusted_quotes` | Mcp Antv Chart List Stock Adjusted Quotes |
| `mcp_antv_chart_list_stock_share_adj_factors` | Mcp Antv Chart List Stock Share Adj Factors |
| `mcp_antv_chart_get_company_profiles` | Mcp Antv Chart Get Company Profiles |
| `mcp_antv_chart_list_stock_income_statements` | Mcp Antv Chart List Stock Income Statements |
| `mcp_antv_chart_list_stock_cash_flows` | Mcp Antv Chart List Stock Cash Flows |
| `mcp_antv_chart_list_stock_balance_sheet` | Mcp Antv Chart List Stock Balance Sheet |
| `mcp_antv_chart_list_stock_earnings_bulletins` | Mcp Antv Chart List Stock Earnings Bulletins |
| `mcp_antv_chart_list_stock_report_schema` | Mcp Antv Chart List Stock Report Schema |
| `mcp_antv_chart_list_stock_holder_cnt` | Mcp Antv Chart List Stock Holder Cnt |
| `mcp_antv_chart_list_stock_major_contracts` | Mcp Antv Chart List Stock Major Contracts |
| `mcp_antv_chart_get_stock_industries` | Mcp Antv Chart Get Stock Industries |
| `mcp_antv_chart_list_stock_executive_shareholding_change` | Mcp Antv Chart List Stock Executive Shareholding Change |
| `mcp_antv_chart_get_stock_margin_securities` | Mcp Antv Chart Get Stock Margin Securities |
| `mcp_antv_chart_list_stock_core_mgmt_changes` | Mcp Antv Chart List Stock Core Mgmt Changes |
| `mcp_antv_chart_list_stock_management_dirs` | Mcp Antv Chart List Stock Management Dirs |
| `mcp_antv_chart_get_stock_rights_issues` | Mcp Antv Chart Get Stock Rights Issues |
| `mcp_antv_chart_list_stock_related_transactions` | Mcp Antv Chart List Stock Related Transactions |
| `mcp_antv_chart_list_resources` | Mcp Antv Chart List Resources |
| `mcp_antv_chart_read_resource` | Mcp Antv Chart Read Resource |
| `mcp_antv_chart_list_prompts` | Mcp Antv Chart List Prompts |
| `mcp_antv_chart_get_prompt` | Mcp Antv Chart Get Prompt |

## 🌐 antv-visual

- **传输方式**: HTTP
- **工具数量**: 25

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_antv_visual_generate_area_chart` | Mcp Antv Visual Generate Area Chart |
| `mcp_antv_visual_generate_bar_chart` | Mcp Antv Visual Generate Bar Chart |
| `mcp_antv_visual_generate_boxplot_chart` | Mcp Antv Visual Generate Boxplot Chart |
| `mcp_antv_visual_generate_column_chart` | Mcp Antv Visual Generate Column Chart |
| `mcp_antv_visual_generate_district_map` | Mcp Antv Visual Generate District Map |
| `mcp_antv_visual_generate_dual_axes_chart` | Mcp Antv Visual Generate Dual Axes Chart |
| `mcp_antv_visual_generate_fishbone_diagram` | Mcp Antv Visual Generate Fishbone Diagram |
| `mcp_antv_visual_generate_flow_diagram` | Mcp Antv Visual Generate Flow Diagram |
| `mcp_antv_visual_generate_funnel_chart` | Mcp Antv Visual Generate Funnel Chart |
| `mcp_antv_visual_generate_histogram_chart` | Mcp Antv Visual Generate Histogram Chart |
| `mcp_antv_visual_generate_line_chart` | Mcp Antv Visual Generate Line Chart |
| `mcp_antv_visual_generate_liquid_chart` | Mcp Antv Visual Generate Liquid Chart |
| `mcp_antv_visual_generate_mind_map` | Mcp Antv Visual Generate Mind Map |
| `mcp_antv_visual_generate_network_graph` | Mcp Antv Visual Generate Network Graph |
| `mcp_antv_visual_generate_organization_chart` | Mcp Antv Visual Generate Organization Chart |
| `mcp_antv_visual_generate_path_map` | Mcp Antv Visual Generate Path Map |
| `mcp_antv_visual_generate_pie_chart` | Mcp Antv Visual Generate Pie Chart |
| `mcp_antv_visual_generate_pin_map` | Mcp Antv Visual Generate Pin Map |
| `mcp_antv_visual_generate_radar_chart` | Mcp Antv Visual Generate Radar Chart |
| `mcp_antv_visual_generate_sankey_chart` | Mcp Antv Visual Generate Sankey Chart |
| `mcp_antv_visual_generate_scatter_chart` | Mcp Antv Visual Generate Scatter Chart |
| `mcp_antv_visual_generate_treemap_chart` | Mcp Antv Visual Generate Treemap Chart |
| `mcp_antv_visual_generate_venn_chart` | Mcp Antv Visual Generate Venn Chart |
| `mcp_antv_visual_generate_violin_chart` | Mcp Antv Visual Generate Violin Chart |
| `mcp_antv_visual_generate_word_cloud_chart` | Mcp Antv Visual Generate Word Cloud Chart |

## 🌐 bmi-mcp

- **传输方式**: HTTP
- **工具数量**: 1

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_bmi_mcp_BMI____` | Mcp Bmi Mcp Bmi     |

## 🌐 bw-ir

- **传输方式**: HTTP
- **工具数量**: 1

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_bw_ir_invoice_verification` | Mcp Bw Ir Invoice Verification |

## 🌐 didi

- **传输方式**: HTTP
- **工具数量**: 13

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_didi_maps_direction_bicycling` | Maps Direction Bicycling |
| `mcp_didi_maps_direction_driving` | Maps Direction Driving |
| `mcp_didi_maps_direction_transit` | Maps Direction Transit |
| `mcp_didi_maps_direction_walking` | Maps Direction Walking |
| `mcp_didi_maps_place_around` | Maps Place Around |
| `mcp_didi_maps_regeocode` | Maps Regeocode |
| `mcp_didi_maps_textsearch` | Maps Textsearch |
| `mcp_didi_taxi_cancel_order` | Taxi Cancel Order |
| `mcp_didi_taxi_create_order` | Taxi Create Order |
| `mcp_didi_taxi_estimate` | Taxi Estimate |
| `mcp_didi_taxi_generate_ride_app_link` | Taxi Generate Ride App Link |
| `mcp_didi_taxi_get_driver_location` | Taxi Get Driver Location |
| `mcp_didi_taxi_query_order` | Taxi Query Order |

## 🔌 doc-forge

- **传输方式**: stdio
- **工具数量**: 16

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_doc_forge_document_reader` | Mcp Doc Forge Document Reader |
| `mcp_doc_forge_pdf_merger` | Mcp Doc Forge Pdf Merger |
| `mcp_doc_forge_pdf_splitter` | Mcp Doc Forge Pdf Splitter |
| `mcp_doc_forge_docx_to_pdf` | Mcp Doc Forge Docx To Pdf |
| `mcp_doc_forge_docx_to_html` | Mcp Doc Forge Docx To Html |
| `mcp_doc_forge_html_cleaner` | Mcp Doc Forge Html Cleaner |
| `mcp_doc_forge_html_to_text` | Mcp Doc Forge Html To Text |
| `mcp_doc_forge_html_to_markdown` | Mcp Doc Forge Html To Markdown |
| `mcp_doc_forge_html_extract_resources` | Mcp Doc Forge Html Extract Resources |
| `mcp_doc_forge_html_formatter` | Mcp Doc Forge Html Formatter |
| `mcp_doc_forge_text_diff` | Mcp Doc Forge Text Diff |
| `mcp_doc_forge_text_splitter` | Mcp Doc Forge Text Splitter |
| `mcp_doc_forge_text_formatter` | Mcp Doc Forge Text Formatter |
| `mcp_doc_forge_text_encoding_converter` | Mcp Doc Forge Text Encoding Converter |
| `mcp_doc_forge_excel_read` | Mcp Doc Forge Excel Read |
| `mcp_doc_forge_format_convert` | Mcp Doc Forge Format Convert |

## 🔌 excel

- **传输方式**: stdio
- **工具数量**: 6

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_excel_excel_copy_sheet` | Excel Copy Sheet |
| `mcp_excel_excel_create_table` | Excel Create Table |
| `mcp_excel_excel_describe_sheets` | Excel Describe Sheets |
| `mcp_excel_excel_format_range` | Excel Format Range |
| `mcp_excel_excel_read_sheet` | Excel Read Sheet |
| `mcp_excel_excel_write_to_sheet` | Excel Write To Sheet |

## 🌐 food-detective

- **传输方式**: HTTP
- **工具数量**: 1

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_food_detective______` | Mcp Food Detective       |

## 🌐 gezhe

- **传输方式**: HTTP
- **工具数量**: 1

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_gezhe_generate_ppt_by_topic` | Generate Ppt By Topic |

## 🔌 github

- **传输方式**: stdio
- **工具数量**: 26

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_github_create_or_update_file` | Create Or Update File |
| `mcp_github_search_repositories` | Search Repositories |
| `mcp_github_create_repository` | Create Repository |
| `mcp_github_get_file_contents` | Get File Contents |
| `mcp_github_push_files` | Push Files |
| `mcp_github_create_issue` | Create Issue |
| `mcp_github_create_pull_request` | Create Pull Request |
| `mcp_github_fork_repository` | Fork Repository |
| `mcp_github_create_branch` | Create Branch |
| `mcp_github_list_commits` | List Commits |
| `mcp_github_list_issues` | List Issues |
| `mcp_github_update_issue` | Update Issue |
| `mcp_github_add_issue_comment` | Add Issue Comment |
| `mcp_github_search_code` | Search Code |
| `mcp_github_search_issues` | Search Issues |
| `mcp_github_search_users` | Search Users |
| `mcp_github_get_issue` | Get Issue |
| `mcp_github_get_pull_request` | Get Pull Request |
| `mcp_github_list_pull_requests` | List Pull Requests |
| `mcp_github_create_pull_request_review` | Create Pull Request Review |
| `mcp_github_merge_pull_request` | Merge Pull Request |
| `mcp_github_get_pull_request_files` | Get Pull Request Files |
| `mcp_github_get_pull_request_status` | Get Pull Request Status |
| `mcp_github_update_pull_request_branch` | Update Pull Request Branch |
| `mcp_github_get_pull_request_comments` | Get Pull Request Comments |
| `mcp_github_get_pull_request_reviews` | Get Pull Request Reviews |

## 🌐 how-to-cook

- **传输方式**: HTTP
- **工具数量**: 5

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_how_to_cook_mcp_howtocook_getAllRecipes` | Mcp How To Cook Mcp Howtocook Getallrecipes |
| `mcp_how_to_cook_mcp_howtocook_getRecipesByCategory` | Mcp How To Cook Mcp Howtocook Getrecipesbycategory |
| `mcp_how_to_cook_mcp_howtocook_recommendMeals` | Mcp How To Cook Mcp Howtocook Recommendmeals |
| `mcp_how_to_cook_mcp_howtocook_whatToEat` | Mcp How To Cook Mcp Howtocook Whattoeat |
| `mcp_how_to_cook_mcp_howtocook_getRecipeById` | Mcp How To Cook Mcp Howtocook Getrecipebyid |

## 🔌 local_time

- **传输方式**: stdio
- **工具数量**: 1

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_local_time_get_current_time` | Get Current Time |

## 🌐 market-cmapi

- **传输方式**: HTTP
- **工具数量**: 2

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_market_cmapi_______` | Mcp Market Cmapi        |
| `mcp_market_cmapi__________` | Mcp Market Cmapi           |

## 🔌 minimax

- **传输方式**: stdio
- **工具数量**: 13

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_minimax_text_to_audio` | Text To Audio |
| `mcp_minimax_list_voices` | List Voices |
| `mcp_minimax_voice_clone` | Voice Clone |
| `mcp_minimax_play_audio` | Play Audio |
| `mcp_minimax_generate_video` | Generate Video |
| `mcp_minimax_query_video_generation` | Query Video Generation |
| `mcp_minimax_text_to_image` | Text To Image |
| `mcp_minimax_music_generation` | Music Generation |
| `mcp_minimax_voice_design` | Voice Design |
| `mcp_minimax_list_resources` | List Resources |
| `mcp_minimax_read_resource` | Read Resource |
| `mcp_minimax_list_prompts` | List Prompts |
| `mcp_minimax_get_prompt` | Get Prompt |

## 🔌 openscad

- **传输方式**: stdio
- **工具数量**: 11

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_openscad_create_3d_model` | Create 3D Model |
| `mcp_openscad_modify_3d_model` | Modify 3D Model |
| `mcp_openscad_export_model` | Export Model |
| `mcp_openscad_list_models` | List Models |
| `mcp_openscad_generate_image` | Generate Image |
| `mcp_openscad_generate_image_gemini` | Generate Image Gemini |
| `mcp_openscad_get_supported_3d_shapes` | Get Supported 3D Shapes |
| `mcp_openscad_list_resources` | List Resources |
| `mcp_openscad_read_resource` | Read Resource |
| `mcp_openscad_list_prompts` | List Prompts |
| `mcp_openscad_get_prompt` | Get Prompt |

## 🔌 pandoc

- **传输方式**: stdio
- **工具数量**: 1

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_pandoc_convert_contents` | Convert Contents |

## 🔌 playwright

- **传输方式**: stdio
- **工具数量**: 12

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_playwright_navigate` | Navigate |
| `mcp_playwright_screenshot` | Screenshot |
| `mcp_playwright_get_page_content` | Get Page Content |
| `mcp_playwright_get_text` | Get Text |
| `mcp_playwright_click` | Click |
| `mcp_playwright_fill` | Fill |
| `mcp_playwright_wait_for_selector` | Wait For Selector |
| `mcp_playwright_close_browser` | Close Browser |
| `mcp_playwright_list_resources` | List Resources |
| `mcp_playwright_read_resource` | Read Resource |
| `mcp_playwright_list_prompts` | List Prompts |
| `mcp_playwright_get_prompt` | Get Prompt |

## 🌐 qrcode-mcp

- **传输方式**: HTTP
- **工具数量**: 1

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_qrcode_mcp______` | Mcp Qrcode Mcp       |

## 🔌 sqlite

- **传输方式**: stdio
- **工具数量**: 5

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_sqlite_read_query` | Read Query |
| `mcp_sqlite_write_query` | Write Query |
| `mcp_sqlite_create_table` | Create Table |
| `mcp_sqlite_list_tables` | List Tables |
| `mcp_sqlite_describe_table` | Describe Table |

## 🌐 stock-quote

- **传输方式**: HTTP
- **工具数量**: 21

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_stock_quote_______` | Mcp Stock Quote        |
| `mcp_stock_quote_____` | Mcp Stock Quote      |
| `mcp_stock_quote_______` | Mcp Stock Quote        |
| `mcp_stock_quote___K_` | Mcp Stock Quote   K  |
| `mcp_stock_quote_A_K_` | Mcp Stock Quote A K  |
| `mcp_stock_quote_____` | Mcp Stock Quote      |
| `mcp_stock_quote_____` | Mcp Stock Quote      |
| `mcp_stock_quote_____` | Mcp Stock Quote      |
| `mcp_stock_quote_A_K___` | Mcp Stock Quote A K    |
| `mcp_stock_quote_A___` | Mcp Stock Quote A    |
| `mcp_stock_quote_A___` | Mcp Stock Quote A    |
| `mcp_stock_quote_____K_` | Mcp Stock Quote     K  |
| `mcp_stock_quote_______` | Mcp Stock Quote        |
| `mcp_stock_quote_______` | Mcp Stock Quote        |
| `mcp_stock_quote_____` | Mcp Stock Quote      |
| `mcp_stock_quote___K_` | Mcp Stock Quote   K  |
| `mcp_stock_quote___K_` | Mcp Stock Quote   K  |
| `mcp_stock_quote_____K_` | Mcp Stock Quote     K  |
| `mcp_stock_quote_____K_` | Mcp Stock Quote     K  |
| `mcp_stock_quote_____` | Mcp Stock Quote      |
| `mcp_stock_quote_______` | Mcp Stock Quote        |

## 🔌 vision-mcp

- **传输方式**: stdio
- **工具数量**: 1

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_vision_mcp_analyze_image` | Mcp Vision Mcp Analyze Image |

## 🔌 weather

- **传输方式**: stdio
- **工具数量**: 3

| 工具名 | 功能说明 |
|--------|----------|
| `mcp_weather_get_weather` | Get Weather |
| `mcp_weather_get_forecast` | Get Forecast |
| `mcp_weather_get_air_quality` | Get Air Quality |

---

*本文档由 Hermes Agent 自动生成
