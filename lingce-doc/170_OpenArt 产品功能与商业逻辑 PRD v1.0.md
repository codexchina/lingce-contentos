# 170_OpenArt 产品功能与商业逻辑 PRD v1.0

版本：v1.0
状态：Product Research / PRD Draft
分析对象：OpenArt
Chrome 打开页面：`https://openart.ai/suite/chat`
补充官网：`https://openart.ai/`
定价页：`https://openart.ai/pricing`
分析日期：2026-09-14
文档定位：拆解 OpenArt 的全栈 AI 创作平台、模型聚合、Director/World/Character/Audio 能力、计费逻辑和可复刻产品设计要点。

---

# 1. 产品概述

OpenArt 是一个 AI 图片、视频、音频和角色创作平台。

一句话定位：

> OpenArt 是将图片、视频、声音、角色、世界和多模型能力整合到一个创作工作室里的 AI Creator Studio。

核心叙事：

```text
One Platform

Infinite Stories

Image + Video + Voice + Audio

All assets generated, edited, and stitched together without leaving the platform
```

---

# 2. 目标用户

核心用户：

* AI 艺术创作者。
* 短视频创作者。
* AI 影视 / MV 制作者。
* 品牌内容团队。
* 虚拟角色 / AI Influencer 运营者。
* 需要多模型统一入口的专业玩家。

---

# 3. 功能清单

## 3.1 创作能力

| 功能 | 功能说明 |
|---|---|
| OpenArt Director | 多场景视频和故事创作工作台 |
| AI Video Generator | 视频生成 |
| AI Image Generator | 图片生成 |
| OpenArt VFX | 视频特效 |
| Video Relight | 视频重打光 |
| Video Background Changer | 视频换背景 |
| OpenArt Worlds | 生成可导航 3D 世界 |
| AI Character | 角色生成和一致性 |
| AI Influencer | AI 虚拟影响者 |
| AI Headshot | 头像生成 |
| AI Face Smooth | 人脸平滑 |
| Smart Shot | 智能镜头 |
| AI Character Swap | 角色替换 |

---

## 3.2 多模态资产

| 类型 | 能力 |
|---|---|
| Image | 生成、编辑、角色、一致性、商品广告 |
| Video | 文生视频、图生视频、特效、换背景、重打光 |
| Character | 一致性角色、虚拟人物、AI Influencer |
| World | Prompt 生成 3D 空间环境 |
| Audio | Voiceover、音乐、音效、口型同步 |
| Model Hub | 聚合多个图像、视频和音频模型 |

官网明确强调聚合多种高级模型，包括 Seedream、Seedance、Google Veo、GPT Image、Sora、Kling、Grok Imagine、MiniMax Hailuo 等。

---

# 4. 用户流程

```text
进入 Suite / Chat

↓

用自然语言描述创作目标

↓

选择或自动路由模型

↓

生成图片、角色、视频、声音或世界

↓

在同一工作室中编辑和组合资产

↓

导出成片 / 图片 / 音频 / 故事资产
```

---

# 5. 定价与计费

OpenArt 采用订阅 + credits + 席位的模式。

公开定价页显示：

| 套餐 | 月价格页面显示 | Credits | 典型能力 |
|---|---|---|---|
| Starter | $13 / Seat / mo 年付折后 | 4,000 / 月 | 约 4,000 图片、约 50 视频、Director、MCP、100+ 模型 |
| Plus | $27 / Seat / mo 年付折后 | 12,000 / 月 | 更大生成量、16 并发、商用权、去水印 |
| Pro | $44 / Seat / mo 年付折后 | 24,000 / 月 | 32 并发、优先支持、更多角色和故事 |
| Wonder | $175 / Seat / mo 年付折后 | 106,000 / 月 | 高额度、Unlimited Creation、优先支持 |

关键商业边界：

* credits 控制生成用量。
* parallel generations 控制速度和生产效率。
* consistent characters、One-Click Stories、personalized models 控制高级创作资产。
* watermark-free 和 commercial use rights 作为付费权益。
* Director、OpenArt MCP、100+ premium models 增加专业用户价值。

---

# 6. 商业逻辑

OpenArt 的商业模式：

```text
多模型聚合

+

创作工作室

+

credits 计费

+

专业创作者订阅

+

高阶故事 / 角色 / 世界能力
```

它的关键不是便宜，而是让用户不用同时订阅多个 AI 模型平台。

---

# 7. 增长闭环

```text
免费开始

↓

用一个 Prompt 生成图片或视频

↓

角色一致性和视频故事提升项目复杂度

↓

用户需要更多 credits、并发和模型

↓

升级 Plus / Pro / Wonder

↓

创作资产沉淀在 OpenArt 工作室
```

---

# 8. 护城河

强护城河：

* 多模型聚合和路由。
* Director 级故事工作台。
* 角色一致性资产。
* Worlds 和 Audio 扩展到完整叙事生产。
* 一站式图片、视频、音频、角色组合。
* 创作者社区和教程生态。

弱护城河：

* 单一文生图。
* 单一图生视频。
* 单一模型接入。
* 普通图片编辑工具。

---

# 9. 风险

* 多模型成本高，credits 规则必须足够清晰。
* 模型版权、商用权和平台责任复杂。
* 全能平台容易变得学习成本高。
* 高阶 Director / Worlds 能力承诺大，失败体验成本高。
* 创作者对输出质量波动非常敏感。

---

# 10. 可复刻 MVP

建议 MVP：

* Chat 创作入口。
* 图片生成。
* 视频生成。
* 角色一致性。
* 模型选择 / 自动路由。
* credits 账户。
* 项目资产库。
* 编辑历史。
* 导出。

V1 增强：

* Director 工作台。
* 多场景故事。
* 音频和口型同步。
* 视频换背景 / 重打光。
* 3D Worlds。
* MCP 或 API。

---

# 11. 结论

OpenArt 的核心价值是“把多个 AI 创作模型变成一个统一 Creator Studio”。

最值得学习的是：

* 用 Chat / Suite 作为统一入口。
* 用 credits 和并发控制商业分层。
* 用角色、故事、世界和音频提高项目粘性。
* 从单次生成走向多资产创作工程。

