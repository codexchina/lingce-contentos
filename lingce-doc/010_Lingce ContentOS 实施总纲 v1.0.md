
# 010_Lingce ContentOS 实施总纲 v1.0

这份文档和 000 的区别：

| 文档       | 解决的问题                              |
| -------- | ---------------------------------- |
| 000 总方案  | Lingce ContentOS 是什么，为什么存在，长期边界是什么 |
| 010 实施总纲 | 第一阶段如何建设，先做什么，后做什么，如何约束开发          |

010 不展开具体类设计和接口设计，而是作为 Codex 开发入口。

---

# 010_Lingce ContentOS 实施总纲 v1.0

## 文档信息

| 项目   | 内容                    |
| ---- | --------------------- |
| 文档名称 | Lingce ContentOS 实施总纲 |
| 文档编号 | 010                   |
| 版本   | v1.0                  |
| 文档类型 | 项目实施规划与工程约束           |
| 所属系统 | Lingce AIOS           |
| 状态   | Baseline              |

---

# 1. 文档定位

本文档定义 Lingce ContentOS 第一阶段及后续阶段的实施路线。

用于指导：

* 产品建设
* 架构演进
* 工程开发
* Agent建设
* Workflow沉淀
* 模型接入
* MVP验证

本文档不定义：

* 具体数据库字段
* 具体接口协议
* 具体代码实现
* 具体模型参数

上述内容由后续专项设计文档定义。

---

# 2. 实施总体原则

## 2.1 以真实内容生产验证系统能力

Lingce ContentOS 第一阶段不是建设完整商业平台。

第一阶段目标：

> 使用 Lingce ContentOS 自身完成真实 AI 内容生产任务。

验证：

* 内容理解能力
* Agent协作能力
* Workflow执行能力
* 模型调度能力
* 资产沉淀能力

---

## 2.2 生产优先，平台后置

实施顺序：

```text
真实生产需求

↓

人工辅助生产

↓

流程固化

↓

Workflow沉淀

↓

系统化编排

↓

产品化
```

禁止：

```text
先开发平台

↓

寻找生产场景
```

---

## 2.3 不追求全自动

第一阶段目标：

不是：

> AI完全替代内容团队。

而是：

> AI承担重复、高耗时、规则明确的生产环节。

保留：

* 人类创意判断
* 内容审核
* 商业决策
* 艺术方向控制

---

# 3. 第一阶段建设目标

## 3.1 总目标

建设：

> Lingce ContentOS Studio v0.1

作为灵策内部 AI 内容生产系统。

---

## 3.2 第一阶段验证任务

完成：

一部 AI 漫剧作品。

形成：

### 一套内容生产流程

包括：

```text
IP输入

↓

剧本生成

↓

分镜生成

↓

角色设计

↓

图片生成

↓

视频生成

↓

配音

↓

剪辑

↓

发布
```

---

### 一套角色资产规范

包括：

* 角色定义
* 参考图
* 风格约束
* 版本管理

---

### 一套 Workflow 模板

包括：

* 角色生成 Workflow
* 场景生成 Workflow
* 分镜生成 Workflow
* 视频生成 Workflow

---

### 一套生产数据记录

包括：

* 时间
* 成本
* 模型
* 参数
* 成功率
* 人工介入点

---

# 4. 第一阶段建设范围

## 4.1 Content Project

目标：

管理内容生产项目。

包含：

* 项目
* IP
* 剧集
* 镜头
* 生产状态

---

## 4.2 Content Asset

目标：

建立内容资产基础。

第一阶段：

重点：

### Character Asset

### Scene Asset

### Style Asset

---

## 4.3 Workflow Management

目标：

管理生产流程。

包括：

* Workflow定义
* Workflow版本
* Workflow参数
* Workflow执行记录

---

## 4.4 Production Task

目标：

统一管理生产任务。

例如：

```text
生成角色图

生成镜头图

生成视频

生成配音
```

---

状态：

```text
PENDING

RUNNING

SUCCESS

FAILED

REVIEW
```

---

# 5. Agent建设路线

第一阶段不建设完整 Agent 体系。

采用渐进方式。

---

## Phase 1.1

基础 Agent：

### Writer Agent

负责：

* 剧本生成
* 分集设计

---

### Storyboard Agent

负责：

* 分镜结构化
* Prompt生成

---

### Production Agent

负责：

* 调度 Workflow
* 调用生产能力

---

### Review Agent

负责：

* 基础质量检查

---

## Phase 1.2

扩展：

* Director Agent
* Character Agent
* Publish Agent

---

# 6. Production Engine 建设路线

## 6.1 原则

Production Engine 不直接绑定模型。

采用：

```text
Production Task

↓

Capability Router

↓

Provider Adapter

↓

External Capability
```

---

## 6.2 第一阶段 Provider

### Image

优先：

* ComfyUI

---

### Video

支持：

* MiniMax H3
* Seedance
* 可灵
* Wan

---

### Audio

支持：

* TTS Provider

---

### Render

支持：

* FFmpeg

---

# 7. ComfyUI 在 ContentOS 中的位置

ComfyUI 定位：

> 视觉生产执行引擎之一。

不是：

* ContentOS核心
* ContentOS产品本身

职责：

负责：

* 图片生成
* 角色一致性流程
* 风格控制
* 部分视频工作流

---

ContentOS负责：

```text
什么时候调用

为什么调用

调用哪个Workflow

输入什么参数

结果如何管理
```

---

# 8. 第一阶段技术路线

## 8.1 Control Plane

负责：

* 项目管理
* Agent管理
* Workflow管理
* 任务管理
* 资产管理

建议：

```text
Java 17

Spring Boot 3

PostgreSQL

Redis

MinIO
```

---

## 8.2 AI Worker

负责：

* AI任务执行
* 模型调用
* 文件处理

建议：

```text
Python

FastAPI

Worker

ComfyUI Client

FFmpeg
```

---

# 9. 第一阶段工程约束

## 9.1 禁止事项

禁止：

### 1. 开发大而全 SaaS

第一阶段不建设：

* 用户体系
* 商城
* 计费
* 多租户

---

### 2. 自研基础模型

不建设：

* 图片模型
* 视频模型
* TTS模型

---

### 3. 模型绑定

禁止：

```text
ContentOS = 某一个模型
```

---

### 4. Workflow不可管理

所有生产流程必须：

* 保存
* 命名
* 版本化
* 可复现

---

# 10. Codex 开发执行规范

Codex 执行开发任务时：

必须遵循：

## 10.1 先文档后代码

流程：

```text
需求确认

↓

设计文档

↓

任务拆解

↓

代码实现

↓

测试

↓

文档更新
```

---

## 10.2 不跨层开发

保持：

```text
Domain

Application

Infrastructure

Adapter

Worker
```

边界清晰。

---

## 10.3 所有 AI 调用必须可追踪

记录：

* Provider
* Model
* Workflow
* Input
* Output
* Cost
* Duration

---

# 11. MVP验收标准

## 内容验收

完成：

* 1个完整内容项目
* 10集以内 AI 漫剧
* 可发布成片

---

## 技术验收

具备：

* 项目管理
* Agent任务执行
* Workflow调用
* 素材管理
* 生产记录

---

## 资产验收

形成：

* 角色库
* Workflow库
* 模型能力库

---

# 12. 后续实施文档

后续：

```text
020_Lingce ContentOS 总体架构设计

030_Lingce ContentOS Content Brain设计

040_Lingce ContentOS Agent Runtime设计

050_Lingce ContentOS Workflow体系设计

060_Lingce ContentOS Production Engine设计

070_Lingce ContentOS Asset体系设计

080_Lingce ContentOS Capability Plane设计

090_Lingce ContentOS Trace与治理设计
```

---

# 13. 最终实施目标

Lingce ContentOS 第一阶段不是建设一个商业平台。

而是完成：

> 从人工 AI 内容探索，到可重复、可管理、可扩展的 AI 内容生产流程迁移。

通过真实内容生产验证系统能力，为后续产品化、商业化和平台化提供基础。
