# 旺旺Agent - API工具文档

> 记录所有可用的MCP（Model Context Protocol）接口

## 更新日期
2026-06-11

---

## 📍 地图与位置

### 高德地图 (amap)
| 工具 | 功能 | 状态 |
|------|------|------|
| maps_geo | 地址→坐标 | ✅ |
| maps_regeocode | 坐标→地址 | ✅ |
| maps_text_search | 关键词搜索POI | ✅ |
| maps_around_search | 周边搜索 | ✅ |
| maps_direction_driving | 驾车路线规划 | ✅ |
| maps_direction_walking | 步行路线规划 | ✅ |
| maps_direction_bicycling | 骑行路线规划 | ✅ |
| maps_direction_transit | 公交路线规划 | ✅ |
| maps_distance | 距离测量 | ✅ |
| maps_weather | 天气预报 | ✅ |
| maps_ip_location | IP定位 | ✅ |

### 滴滴出行 (didi)
| 工具 | 功能 | 状态 |
|------|------|------|
| maps_textsearch | 地点搜索 | ✅ |
| maps_regeocode | 坐标→地址 | ✅ |
| maps_place_around | 周边搜索 | ✅ |
| maps_direction_driving | 驾车路线 | ✅ |
| maps_direction_transit | 公交路线 | ✅ |
| maps_direction_walking | 步行路线 | ✅ |
| maps_direction_bicycling | 骑行路线 | ✅ |
| taxi_estimate | 预估价格 | ✅ |
| taxi_create_order | 创建订单 | ✅ |
| taxi_query_order | 查询订单 | ✅ |
| taxi_cancel_order | 取消订单 | ✅ |
| taxi_get_driver_location | 司机位置 | ✅ |
| taxi_generate_ride_app_link | 生成打车链接 | ✅ |

---

## 📊 金融数据

### 股票行情 (stock-quote)
- A股K线（1分钟/日/周/月）
- 外汇报价
- 全球指数

### 金融图表 (antv-chart)
| 类别 | 功能 |
|------|------|
| 股票数据 | 公司信息、行业分类、利润表、资产负债表等 |
| 基金数据 | 净值、持仓、管理人、费率等 |
| 指数数据 | 历史行情、成分股 |
| 宏观数据 | CPI、PPI、货币供应量、社融、国债收益率 |

---

## 🎨 内容生成

### 图片生成
- OpenAI GPT-Image-2（默认，效果最佳）
- MiniMax 图片生成（备用）

### 视频生成
- MiniMax 视频生成

### 语音合成
- MiniMax TTS（支持中文、多种音色）

### 二维码生成 (qrcode-mcp)
- 生成二维码图片

---

## 🛠️ 工具类

### OpenSCAD 3D建模
- create_3d_model - 自然语言生成3D模型
- export_model - 导出STL等格式

### PDF处理
- PDF阅读、转换、合并、分割

### Excel处理
- 读取、写入、格式化表格

### OCR文档识别
- 文字识别、文档解析

---

## 🌐 搜索与爬虫

### Firecrawl
- 网页搜索、抓取、深度研究

### Playwright
- 浏览器自动化

---

## 🎯 其他

### 12306火车票
- 余票查询、预订、改签、退票

### 瑞幸咖啡
- ⚠️ Token过期，待修复

### 小红书
- 笔记搜索、详情获取

### 美食推荐
- 各地美食推荐

---

## 📝 使用示例

### 叫车
```
用户：帮我从上川去华强北打车
1. 搜索起点终点坐标
2. taxi_estimate 预估价格
3. 用户选择车型
4. taxi_create_order 下单
```

### 地图查询
```
用户：帮我查一下深圳欢乐谷在哪
→ maps_geo 返回坐标和地址
```

### 股票查询
```
用户：查一下茅台的股价
→ stock-quote 返回实时行情
```

---

*本文档由旺旺Agent自动生成*
