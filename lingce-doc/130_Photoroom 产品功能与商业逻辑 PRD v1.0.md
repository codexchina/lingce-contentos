# 130_Photoroom 产品功能与商业逻辑 PRD v1.0

版本：v1.0
状态：Product Research / PRD Draft
分析对象：Photoroom
Chrome 打开页面：`https://app.photoroom.com/create`
补充官网：`https://www.photoroom.com/`
定价页：`https://www.photoroom.com/pricing`
分析日期：2026-09-14
文档定位：拆解 Photoroom 的产品功能、商品图工作流、计费结构、商业逻辑和可复刻产品设计要点。

---

# 1. 产品概述

Photoroom 是面向电商商品视觉的 AI 图片编辑和 Listing Studio。

一句话定位：

> Photoroom 是帮助商家快速生成专业商品图、背景、模特图和多平台上架素材的 AI 商品视觉生产平台。

它的核心不是通用修图，而是围绕商品照片的标准化处理：

```text
商品原图

↓

抠图 / 背景 / 阴影 / 修复

↓

品牌模板

↓

批量处理

↓

导出 / 上架 / API 自动化
```

---

# 2. 目标用户

核心用户：

* 独立电商卖家。
* Shopify、Amazon、Etsy 等平台商家。
* 品牌电商团队。
* 大商品目录运营团队。
* Marketplace 和平台型客户。
* 需要 API 批处理的企业。

---

# 3. 功能清单

## 3.1 核心工具

| 功能 | 功能说明 |
|---|---|
| Background Remover | 快速去背景 |
| Retouch | 局部修图和瑕疵处理 |
| AI Product Fixer | 商品图修复 |
| AI Shadows | 添加真实阴影 |
| AI Fill | 生成式填充 |
| AI Expand / Resize | 扩图和尺寸适配 |
| Image Enhancer | 图片增强 |
| AI Backgrounds | 生成商品背景 |
| AI Product Photography | 生成专业商品摄影图 |
| AI Fashion Models | 生成服装模特图 |
| Video Templates | 用商品图生成短视频模板 |
| Brand Kit | 管理品牌颜色、Logo、布局 |
| Spaces | 团队协作空间 |
| Shopify Integration | Shopify 集成 |
| Image API | 自动化图片处理接口 |
| Marketplace Sync | 同步到 Shopify 和 Marketplace feed |

---

## 3.2 批量与企业能力

| 能力 | 说明 |
|---|---|
| Batch Edit | 通过 Web App 或 API 批量处理上千张图 |
| Dedicated capacity | 企业专用容量 |
| Custom endpoints | 企业定制 API |
| SLA | 企业级可用性保障 |
| SOC 2 Type 2 | 企业安全合规背书 |
| Visual QA | 企业视觉质检 |
| ROI data | 视觉效果和商业回报数据 |

---

# 4. 用户流程

```text
上传商品照片

↓

自动识别商品主体

↓

去背景 / 修复 / 阴影

↓

选择背景或品牌模板

↓

批量应用到 SKU

↓

导出多尺寸素材

↓

同步到店铺或广告平台
```

---

# 5. 定价与商业逻辑

Photoroom 采用订阅 + AI credits + 导出额度 + 企业定制的模式。

公开定价结构：

| 套餐 | 定位 | AI credits | Exports |
|---|---|---|---|
| Pro | 个体创业者 | 8,000 / 月 | 1,000 / 月 |
| Max | 小企业 | 25,000 / 月 | 3,000 / 月 |
| Ultra | 成长品牌 / 大目录 | 75,000 / 月 | 10,000 / 月 |
| Enterprise | 大客户 | Custom | Custom |

能力限制体现商业分层：

* Pro 包含核心工具，但不含 Video Generator、4K 视频/图片分辨率。
* Max 开始支持 Video Generator 和 Shopify Integration。
* Ultra 支持更高生成量和 4K 输出。
* Enterprise 提供视觉 QA、视觉专家、ROI 数据、SLA、SSO、专属支持。

---

# 6. 商业闭环

```text
免费试用吸引商家

↓

核心抠图和商品图工具建立刚需

↓

SKU 数量增长带来批量需求

↓

AI credits 和 exports 形成用量限制

↓

团队协作、Shopify 集成、API 推动升级

↓

企业客户购买 SLA、定制容量和视觉 QA
```

---

# 7. 护城河

强护城河：

* 商品图垂直场景极深。
* 从个体卖家到企业 API 的完整分层。
* 批量处理和 API 自动化能力。
* 品牌模板、空间协作和 Marketplace Sync。
* 商品主体识别、阴影、背景、视觉 QA 的链路组合。

弱护城河：

* 单一抠图能力。
* 单一 AI 背景生成。
* 普通图片增强。

---

# 8. 风险

* AI credits 和 exports 双限制会增加理解成本。
* 视频能力相对图片能力不是核心心智。
* 企业能力强，但中小商家可能只使用免费和低价工具。
* Shopify 等集成依赖外部平台策略。

---

# 9. 可复刻 MVP

建议 MVP：

* 商品图上传。
* 自动抠图。
* 背景生成。
* 阴影生成。
* 商品图模板。
* 批量处理。
* 导出额度。
* 品牌 Kit。
* 历史项目。

进一步版本：

* Shopify 集成。
* API 批处理。
* AI Fashion Models。
* 视频模板。
* 视觉 QA。

---

# 10. 结论

Photoroom 的核心不是“AI 修图”，而是“商品视觉生产基础设施”。

最值得学习的是：

* 把低频设计变成高频 SKU 工作流。
* 用批量、导出和 credits 做商业计量。
* 用企业 API 和视觉 QA 拉高客单价。
* 从工具层走向上架和渠道同步层。

