# 150_Pippit 产品功能与商业逻辑 PRD v1.0

版本：v1.0
状态：Product Research / PRD Draft
分析对象：Pippit
Chrome 打开页面：`https://www.pippit.ai/home`
补充官网：`https://www.pippit.ai/`
定价页：`https://www.pippit.ai/pricing`
分析日期：2026-09-14
文档定位：拆解 Pippit 的 Smart Creative Agent、视频/图片/Avatar/发布平台能力、计费逻辑和可复刻产品设计要点。

---

# 1. 产品概述

Pippit 是一个 AI 内容创作平台，官网将其定义为 Smart Creative Agent。

一句话定位：

> Pippit 是面向创作者、营销人员和商家的 AI 创意代理，负责从链接、素材或提示词生成视频、图片、Avatar 内容并支持发布运营。

它的产品关键词是：

```text
Agent

Video

Image

Avatar

Story Studio

Assets

Publisher

Analytics
```

---

# 2. 目标用户

核心用户：

* 内容创作者。
* 营销人员。
* 商家和中小企业。
* 教育者。
* 社交媒体运营。
* 短剧、短片、AI 影视创作者。

---

# 3. 功能清单

## 3.1 AI Features

| 功能 | 说明 |
|---|---|
| Video Agent | 视频创作代理 |
| AI Image Generator | AI 图片生成 |
| AI Design | AI 设计 |
| AI Avatar | AI Avatar |
| AI Talking Photo | 会说话照片 |

---

## 3.2 AI Models

| 模型 | 说明 |
|---|---|
| Seedance 2.5 | 视频生成模型 |
| Seedream | 图像生成模型 |
| Sora 2 | 视频模型 |
| Seedance | 视频模型 |
| Nano Banana Pro | 图片生成 / 编辑模型 |

---

## 3.3 Story Studio

| 功能 | 说明 |
|---|---|
| AI Drama | AI 短剧 |
| AI Film | AI 影片 |
| AI Movie | AI 电影 |
| AI Script | AI 剧本 |
| AI Workflow | AI 工作流 |

---

## 3.4 产品工具

| 分类 | 工具 |
|---|---|
| Video Generator | AI Video Generator、Image to Video、AI UGC、Video Translator、Product Showcase |
| Image | AI Design、AI Background、Layout to Design、Image Resizer、Upscale Image |
| Avatars | Digital Avatar、Custom Avatar、Custom Voices、Prompt to Avatar、AI Dubbing |
| Platform | Data Analytics、Schedule Posting、Content Publisher、Assets Management |

---

# 4. 用户流程

视频生成流程：

```text
进入 Pippit

↓

选择视频模型或 Video Agent

↓

上传链接、媒体或文件作为参考

↓

输入创作提示词

↓

设置比例、语言和时长

↓

生成视频

↓

继续对话修改或创建下一个视频
```

图片生成流程：

```text
选择 Create image

↓

输入图片描述

↓

选择比例

↓

生成多张图片

↓

混合、合并、换背景或去背景
```

---

# 5. 定价与计费

Pippit 采用免费入口 + 订阅套餐 + credits 的模式。

公开定价页显示：

| 套餐 | 年付价格页面显示 | Credits | 典型权益 |
|---|---|---|---|
| Free | GBP0 | 免费每日 credits | Video Agent、Remix viral videos、Talking photos、Image Agent |
| Starter | GBP90 / Yearly | 2,100 credits / 月 | 买 credits、快速生成、高级模型、去水印 |
| Plus | GBP265 / Yearly | 6,700 credits / 月 | 更快生成、高级模型、去水印 |
| Pro | GBP1,330 / Yearly | 35,500 credits / 月 | 最快生成、高级模型、去水印 |

Plan Details 中还包含：

* Link to video。
* Marketing holiday video & poster generator。
* Smart crop。
* Video editor。
* Remove background。
* Custom voices。
* Avatar video。
* Image studio。
* Product photos。
* Sales poster。
* Batch edit。
* Assets。
* 商用模板和免费商用素材。

---

# 6. 商业逻辑

Pippit 的商业逻辑是：

```text
免费 credits 让用户试用

↓

Agent 降低内容创作门槛

↓

视频、图片、Avatar 覆盖多内容形态

↓

高级模型、去水印、速度和 credits 推动付费

↓

发布、排程、数据分析提升平台粘性
```

与单点视频生成工具相比，Pippit 更想做“内容生产和发布操作台”。

---

# 7. 护城河

强护城河：

* 字节 / CapCut 生态心智。
* Video Agent 与多模型整合。
* 从生成到编辑、发布、数据分析的闭环。
* Story Studio 对短剧、电影、剧本的高阶场景覆盖。
* 免费 credits 和去水印付费的清晰转化路径。

弱护城河：

* 单一文生视频。
* 单一图生视频。
* 简单图片生成。
* 单一去背景能力。

---

# 8. 风险

* 功能过多，普通用户可能不知道从哪里开始。
* 高级视频模型成本高，credits 规则需要足够透明。
* Story Studio 的承诺很大，稳定生成长内容难度高。
* 发布和数据分析能力需要深度连接外部平台。
* 多模型聚合需要处理质量差异、版权和可商用边界。

---

# 9. 可复刻 MVP

建议 MVP：

* Video Agent。
* 链接 / 文件 / 文本生成视频。
* 图片生成。
* Avatar 口播。
* 去水印付费权益。
* credits 账户。
* 任务历史。
* 内容资产库。
* 简单发布排程。

V1 增强：

* Story Studio。
* 视频翻译。
* 自定义声音。
* 数据分析。
* 多平台内容 Publisher。
* 团队空间。

---

# 10. 结论

Pippit 的价值在于把 AI 生成器包装成 Creative Agent。

最值得学习的是：

* 用 Agent 对话承接创作意图。
* 用免费 credits 建立试用。
* 用去水印、速度和高级模型做付费边界。
* 把发布、排程、数据分析纳入内容生产闭环。

