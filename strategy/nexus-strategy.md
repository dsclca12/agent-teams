# 🌐 NEXUS —— 专家网络，战略统一

## Agency 多 Agent 编排的完整操作 Playbook

> **NEXUS** 将 Agency 的独立 AI 专家转变为同步的智能网络。这不是一个提示词集合 —— 它是一个**部署规范**，将 Agency 转变为任何项目、产品或组织的力量倍增器。

---

## 目录

1. [战略基础](#1-战略基础)
2. [NEXUS 运营模式](#2-the-nexus-operating-model)
3. [Phase 0 —— 情报与发现](#3-phase-0--intelligence--discovery)
4. [Phase 1 —— 战略与架构](#4-phase-1--strategy--architecture)
5. [Phase 2 —— 基础与脚手架](#5-phase-2--foundation--scaffolding)
6. [Phase 3 —— 构建与迭代](#6-phase-3--build--iterate)
7. [Phase 4 —— 质量与加固](#7-phase-4--quality--hardening)
8. [Phase 5 —— 发布与增长](#8-phase-5--launch--growth)
9. [Phase 6 —— 运营与演进](#9-phase-6--operate--evolve)
10. [Agent 协调矩阵](#10-agent-coordination-matrix)
11. [交接协议](#11-handoff-protocols)
12. [质量门控](#12-quality-gates)
13. [风险管理](#13-risk-management)
14. [成功指标](#14-success-metrics)
15. [快速入门激活指南](#15-quick-start-activation-guide)

---

## 1. 战略基础

### 1.1 NEXUS 解决的问题

单个 Agent 很强大。但缺乏协调时，它们会产生：
- 冲突的架构决策
- 跨部门的重复工作
- 交接边界的质量差距
- 没有共享上下文或机构记忆

**NEXUS 消除了这些失败模式**，通过定义：
- **谁** 在每个阶段激活
- **生产什么** 以及为谁生产
- **何时** 交接以及交给谁
- **如何** 在推进前验证质量
- **为什么** 每个 Agent 存在于流水线中（没有乘客）

### 1.2 核心原则

| 原则 | 描述 |
|------|------|
| **流水线完整性** | 没有通过质量门控，任何阶段都不能推进 |
| **上下文连续性** | 每次交接都携带完整上下文 —— 任何 Agent 都不会冷启动 |
| **并行执行** | 独立工作流同时运行以压缩时间线 |
| **证据胜于声明** | 所有质量评估都需要证明，而非断言 |
| **快速失败，快速修复** | 每个任务最多 3 次重试后升级 |
| **单一事实来源** | 一个规范文档、一个任务列表、一个架构文档 |

### 1.3 按部门划分的 Agent 名册

| 部门 | Agent | 主要 NEXUS 角色 |
|------|-------|----------------|
| **Engineering** | Frontend Developer、Backend Architect、Mobile App Builder、AI Engineer、DevOps Automator、Rapid Prototyper、Senior Developer | 构建、部署和维护所有技术系统 |
| **Design** | UI Designer、UX Researcher、UX Architect、Brand Guardian、Visual Storyteller、Whimsy Injector、Image Prompt Engineer | 定义视觉标识、用户体验和品牌一致性 |
| **Marketing** | Growth Hacker、Content Creator、Twitter Engager、TikTok Strategist、Instagram Curator、Reddit Community Builder、App Store Optimizer、Social Media Strategist | 推动获客、参与度和市场存在 |
| **Product** | Sprint Prioritizer、Trend Researcher、Feedback Synthesizer | 定义构建什么、何时构建、为何构建 |
| **Project Management** | Studio Producer、Project Shepherd、Studio Operations、Experiment Tracker、Senior Project Manager | 编排时间线、资源和跨职能协调 |
| **Testing** | Evidence Collector、Reality Checker、Test Results Analyzer、Performance Benchmarker、API Tester、Tool Evaluator、Workflow Optimizer | 通过基于证据的评估验证质量 |
| **Support** | Support Responder、Analytics Reporter、Finance Tracker、Infrastructure Maintainer、Legal Compliance Checker、Executive Summary Generator | 维持运营、合规和商业智能 |
| **Spatial Computing** | XR Interface Architect、macOS Spatial/Metal Engineer、XR Immersive Developer、XR Cockpit Interaction Specialist、visionOS Spatial Engineer、Terminal Integration Specialist | 构建沉浸式和空间计算体验 |
| **Specialized** | Agents Orchestrator、Data Analytics Reporter、LSP/Index Engineer、Sales Data Extraction Agent、Data Consolidation Agent、Report Distribution Agent | 跨领域协调、深度分析和代码智能 |

---

## 2. NEXUS 运营模式

### 2.1 七阶段流水线

```
┌─────────────────────────────────────────────────────────────────────────┐
│                        NEXUS 流水线                                     │
│                                                                         │
│  Phase 0        Phase 1         Phase 2          Phase 3                │
│  发现     ───▶ 战略     ───▶ 基础     ───▶  构建                 │
│  情报           架构            脚手架          Dev ↔ QA 循环           │
│                                                                         │
│  Phase 4        Phase 5         Phase 6                                 │
│  加固     ───▶  发布     ───▶  运营                                │
│  质量门控       上市             持续运营                                │
│                                                                         │
│  ◆ 每个阶段之间都有质量门控                                              │
│  ◆ 阶段内有并行轨道                                                      │
│  ◆ 每个边界都有反馈循环                                                  │
└─────────────────────────────────────────────────────────────────────────┘
```

### 2.2 指挥结构

```
                    ┌──────────────────────┐
                    │  Agents Orchestrator  │  ◄── 流水线控制器
                    │  (Specialized)        │
                    └──────────┬───────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
     ┌────────▼──────┐ ┌──────▼───────┐ ┌──────▼──────────┐
     │ Studio        │ │ Project      │ │ Senior Project   │
     │ Producer      │ │ Shepherd     │ │ Manager          │
     │ (组合管理)    │ │ (执行管理)   │ │ (任务界定)       │
     └───────────────┘ └──────────────┘ └─────────────────┘
              │                │                │
              ▼                ▼                ▼
     ┌─────────────────────────────────────────────────┐
     │           部门负责人（每个阶段）                  │
     │  Engineering │ Design │ Marketing │ Product │ QA │
     └─────────────────────────────────────────────────┘
```

### 2.3 激活模式

NEXUS 支持三种部署配置：

| 模式 | 活跃 Agent 数量 | 使用场景 | 时间线 |
|------|----------------|----------|--------|
| **NEXUS-Full** | 全部 | 企业产品发布，完整生命周期 | 12-24 周 |
| **NEXUS-Sprint** | 15-25 | 功能开发，MVP 构建 | 2-6 周 |
| **NEXUS-Micro** | 5-10 | Bug 修复、内容活动、单一交付物 | 1-5 天 |

---

## 3. Phase 0 —— 情报与发现

> **目标**：在投入资源之前了解情况。在验证问题之前不进行构建。

### 3.1 活跃 Agent

| Agent | 阶段角色 | 主要输出 |
|-------|---------|---------|
| **Trend Researcher** | 市场情报负责人 | 市场分析报告（含 TAM/SAM/SOM） |
| **Feedback Synthesizer** | 用户需求分析 | 包含痛点的综合反馈报告 |
| **UX Researcher** | 用户行为分析 | 包含用户画像和旅程图的研究发现 |
| **Analytics Reporter** | 数据领域评估 | 包含可用信号的数据审计报告 |
| **Legal Compliance Checker** | 法规扫描 | 合规要求矩阵 |
| **Tool Evaluator** | 技术领域评估 | 技术栈评估 |

### 3.2 并行工作流

```
工作流 A：市场情报                    工作流 B：用户情报
├── Trend Researcher                  ├── Feedback Synthesizer
│   ├── 竞争格局                      │   ├── 多渠道反馈收集
│   ├── 市场规模估算（TAM/SAM/SOM）   │   ├── 情感分析
│   └── 趋势生命周期映射              │   └── 痛点优先级排序
│                                     │
├── Analytics Reporter                ├── UX Researcher
│   ├── 现有数据审计                  │   ├── 用户访谈/调研
│   ├── 信号识别                      │   ├── 用户画像开发
│   └── 基线指标                      │   └── 旅程映射
│                                     │
└── Legal Compliance Checker          └── Tool Evaluator
    ├── 法规要求                          ├── 技术评估
    ├── 数据处理约束                       ├── 自建 vs 购买分析
    └── 管辖区映射                         └── 集成可行性
```

### 3.3 Phase 0 质量门控

**门控负责人**：Executive Summary Generator

| 标准 | 阈值 | 所需证据 |
|------|------|---------|
| 市场机会已验证 | TAM > 最低可行阈值 | Trend Researcher 报告及来源 |
| 用户需求已确认 | ≥3 个已验证的痛点 | Feedback Synthesizer + UX Researcher 数据 |
| 法规路径清晰 | 没有阻塞性合规问题 | Legal Compliance Checker 矩阵 |
| 数据基础已评估 | 关键指标已识别 | Analytics Reporter 审计 |
| 技术可行性已确认 | 技术栈已验证 | Tool Evaluator 评估 |

**输出**：执行摘要（≤500 字，SCQA 格式）→ 决策：GO / NO-GO / PIVOT

---

## 4. Phase 1 —— 战略与架构

> **目标**：定义我们要构建什么、如何构建、成功是什么样的 —— 在编写任何代码之前。

### 4.1 活跃 Agent

| Agent | 阶段角色 | 主要输出 |
|-------|---------|---------|
| **Studio Producer** | 战略组合对齐 | 战略组合计划 |
| **Senior Project Manager** | 规格转任务 | 综合任务列表 |
| **Sprint Prioritizer** | 功能优先级排序 | 优先级 Backlog（RICE 评分） |
| **UX Architect** | 技术架构 + UX 基础 | 架���规范 + CSS 设计系统 |
| **Brand Guardian** | 品牌标识系统 | 品牌基础文档 |
| **Backend Architect** | 系统架构 | 系统架构规范 |
| **AI Engineer** | AI/ML 架构（如适用） | ML 系统设计 |
| **Finance Tracker** | 预算和资源规划 | 财务计划及 ROI 预测 |

### 4.2 执行序列

```
步骤 1：战略框架（并行）
├── Studio Producer → 战略组合计划（愿景、目标、ROI 目标）
├── Brand Guardian → 品牌基础（宗旨、价值观、视觉标识系统）
└── Finance Tracker → 预算框架（资源分配、成本预测）

步骤 2：技术架构（并行，步骤 1 之后）
├── UX Architect → CSS 设计系统 + 布局框架 + UX 结构
├── Backend Architect → 系统架构（服务、数据库、API）
├── AI Engineer → ML 架构（模型、流水线、推理策略）
└── Senior Project Manager → 任务列表（规格 → 任务，精确需求）

步骤 3：优先级排序（顺序，步骤 2 之后）
└── Sprint Prioritizer → RICE 评分的 backlog 及冲刺分配
    ├── 输入：任务列表 + 架构规范 + 预算框架
    ├── 输出：带依赖图的优先冲刺计划
    └── 验证：Studio Producer 确认战略对齐
```

### 4.3 Phase 1 质量门控

**门控负责人**：Studio Producer + Reality Checker（双重签核）

| 标准 | 阈值 | 所需证据 |
|------|------|---------|
| 架构覆盖所有需求 | 100% 规格覆盖 | Senior PM 任务列表交叉引用 |
| 品牌系统完整 | Logo、颜色、排版、语调已定义 | Brand Guardian 交付物 |
| 技术可行性已验证 | 所有组件都有实现路径 | Backend Architect + UX Architect 规范 |
| 预算已批准 | 在组织约束范围内 | Finance Tracker 计划 |
| 冲刺计划现实可行 | 基于速度的估算 | Sprint Prioritizer backlog |

**输出**：已批准的架构包 → Phase 2 激活

---

## 5. Phase 2 —— 基础与脚手架

> **目标**：构建所有后续工作依赖的技术和运营基础。在添加肌肉之前让骨架先站立起来。

### 5.1 活跃 Agent

| Agent | 阶段角色 | 主要输出 |
|-------|---------|---------|
| **DevOps Automator** | CI/CD 流水线 + 基础设施 | 部署流水线 + IaC 模板 |
| **Frontend Developer** | 项目脚手架 + 组件库 | 应用骨架 + 设计系统实现 |
| **Backend Architect** | 数据库 + API 基础 | Schema + API 脚手架 + 认证系统 |
| **UX Architect** | CSS 系统实现 | 设计令牌 + 布局框架 |
| **Infrastructure Maintainer** | 云基础设施设置 | 监控 + 日志 + 告警 |
| **Studio Operations** | 流程设置 | 协作工具 + 工作流 |

### 5.2 并行工作流

```
工作流 A：基础设施                  工作流 B：应用基础
├── DevOps Automator                ├── Frontend Developer
│   ├── CI/CD 流水线（GitHub Actions）  │   ├── 项目脚手架
│   ├── 容器编排                      │   ├── 组件库设置
│   └── 环境配置                      │   └── 设计系统集成
│                                   │
├── Infrastructure Maintainer       ├── Backend Architect
│   ├── 云资源配置                    │   ├── 数据库 schema 部署
│   ├── 监控（Prometheus/Grafana）    │   ├── API 脚手架 + 认证
│   └── 安全加固                      │   └── 服务通信层
│                                   │
└── Studio Operations               └── UX Architect
    ├── Git 工作流 + 分支策略            ├── CSS 设计令牌
    ├── 沟通渠道                        ├── 响应式布局系统
    └── 文档模板                        └── 主题系统（浅色/深色/系统）
```

### 5.3 Phase 2 质量门控

**门控负责人**：DevOps Automator + Evidence Collector

| 标准 | 阈值 | 所需证据 |
|------|------|---------|
| CI/CD 流水线可运行 | 构建 + 测试 + 部署工作正常 | 流水线执行日志 |
| 数据库 schema 已部署 | 所有表/索引已创建 | 迁移成功 + schema 导出 |
| API 脚手架响应正常 | 健康检查端点存活 | curl 响应截图 |
| 前端渲染正常 | 骨架应用在浏览器中加载 | Evidence Collector 截图 |
| 监控已激活 | 仪表板显示指标 | Grafana/监控截图 |
| 设计系统已实现 | 令牌 + 组件可用 | 组件库演示 |

**输出**：可运行的骨架应用及完整 DevOps 流水线 → Phase 3 激活

---

## 6. Phase 3 —— 构建与迭代

> **目标**：通过持续的 Dev↔QA 循环实现功能。每个任务在下一个任务开始前都要验证。这是大部分工作发生的地方。

### 6.1 Dev↔QA 循环

这是 NEXUS 的核心。Agents Orchestrator 管理**逐任务质量循环**：

```
┌─────────────────────────────────────────────────────────┐
│                   DEV ↔ QA 循环                         │
│                                                         │
│  ┌──────────┐    ┌──────────┐    ┌──────────────────┐   │
│  │ Developer │───▶│ Evidence │───▶│ 决策逻辑          │   │
│  │ Agent     │    │ Collector│    │                   │   │
│  │           │    │ (QA)     │    │ PASS ��� 下一任务   │   │
│  │ 实现任务 N│    │          │    │ FAIL → 重试（≤3）│   │
│  │           │◀───│ 测试任务 N│◀───│ BLOCKED → 升级   │   │
│  └──────────┘    └──────────┘    └──────────────────┘   │
│       ▲                                    │             │
│       │            QA 反馈                 │             │
│       └────────────────────────────────────┘             │
│                                                         │
│  Orchestrator 跟踪：尝试次数、QA 反馈、                   │
│  任务状态、累积质量指标                                    │
└─────────────────────────────────────────────────────────┘
```

### 6.2 按任务类型的 Agent 分配

| 任务类型 | 主要开发者 | QA Agent | 专家支持 |
|---------|-----------|----------|---------|
| Frontend UI | Frontend Developer | Evidence Collector | UI Designer、Whimsy Injector |
| Backend API | Backend Architect | API Tester | Performance Benchmarker |
| Database | Backend Architect | API Tester | Analytics Reporter |
| Mobile | Mobile App Builder | Evidence Collector | UX Researcher |
| AI/ML Feature | AI Engineer | Test Results Analyzer | Data Analytics Reporter |
| Infrastructure | DevOps Automator | Performance Benchmarker | Infrastructure Maintainer |
| 高级打磨 | Senior Developer | Evidence Collector | Visual Storyteller |
| 快速原型 | Rapid Prototyper | Evidence Collector | Experiment Tracker |
| Spatial/XR | XR Immersive Developer | Evidence Collector | XR Interface Architect |
| visionOS | visionOS Spatial Engineer | Evidence Collector | macOS Spatial/Metal Engineer |
| Cockpit UI | XR Cockpit Interaction Specialist | Evidence Collector | XR Interface Architect |
| CLI/Terminal | Terminal Integration Specialist | API Tester | LSP/Index Engineer |
| Code Intelligence | LSP/Index Engineer | Test Results Analyzer | Senior Developer |

### 6.3 并行构建轨道

对于复杂项目，多个轨道同时运行：

```
轨道 A：核心产品                    轨道 B：增长与营销
├── Frontend Developer              ├── Growth Hacker
│   └── UI 实现                     │   └── 病毒循环 + 推荐系统
├── Backend Architect               ├── Content Creator
│   └── API + 业务逻辑              │   └── 发布内容 + 编辑日历
├── AI Engineer                     ├── Social Media Strategist
│   └── ML 功能 + 流水线            │   └── 跨平台活动
│                                   ├── App Store Optimizer（如移动端）
│                                   │   └── ASO 策略 + 元数据
│                                   │
轨道 C：质量与运营                  轨道 D：品牌与体验
├── Evidence Collector              ├── UI Designer
│   └── 持续 QA 截图                │   └── 组件优化
├── API Tester                      ├── Brand Guardian
│   └── 端点验证                    │   └── 品牌一致性审计
├── Performance Benchmarker         ├── Visual Storyteller
│   └── 负载测试 + 优化             │   └── 视觉叙事资产
├── Workflow Optimizer              └── Whimsy Injector
│   └── 流程改进                        └── 愉悦时刻 + 微交互
└── Experiment Tracker
    └── A/B 测试管理
```

### 6.4 Phase 3 质量门控

**门控负责人**：Agents Orchestrator

| 标准 | 阈值 | 所需证据 |
|------|------|---------|
| 所有任务通过 QA | 100% 任务完成 | Evidence Collector 每任务截图 |
| API 端点已验证 | 所有端点已测试 | API Tester 报告 |
| 性能基线达标 | P95 < 200ms，LCP < 2.5s | Performance Benchmarker 报告 |
| 品牌一致性已验证 | 95%+ 符合度 | Brand Guardian 审计 |
| 无严重 Bug | 零 P0/P1 未解决问题 | Test Results Analyzer 摘要 |

**输出**：功能完整的应用 → Phase 4 激活

---

## 7. Phase 4 —— 质量与加固

> **目标**：最终质量考验。Reality Checker 默认"需要修改" —— 你必须用压倒性的证据证明生产就绪。

### 7.1 活跃 Agent

| Agent | 阶段角色 | 主要输出 |
|-------|---------|---------|
| **Reality Checker** | 最终集成测试（默认需要修改） | 基于现实的集成报告 |
| **Evidence Collector** | 全面视觉证据 | 截图证据包 |
| **Performance Benchmarker** | 负载测试 + 优化 | 性能认证 |
| **API Tester** | 完整 API 回归套件 | API 测试报告 |
| **Test Results Analyzer** | 聚合质量指标 | 质量指标仪表板 |
| **Legal Compliance Checker** | 最终合规审计 | 合规认证 |
| **Infrastructure Maintainer** | 生产就绪检查 | 基础设施就绪报告 |
| **Workflow Optimizer** | 流程效率审查 | 优化建议 |

### 7.2 加固序列

```
步骤 1：证据收集（并行）
├── Evidence Collector → 完整截图套件（桌面、平板、移动端）
├── API Tester → 完整端点回归
├── Performance Benchmarker → 10 倍预期流量负载测试
└── Legal Compliance Checker → 最终法规审计

步骤 2：分析（并��，步骤 1 之后）
├── Test Results Analyzer → 将所有测试数据聚合到质量仪表板
├── Workflow Optimizer → 识别剩余的流程低效问题
└── Infrastructure Maintainer → 生产环境验证

步骤 3：最终裁决（顺序，步骤 2 之后）
└── Reality Checker → 集成报告
    ├── 交叉验证所有之前的 QA 发现
    ├── 用截图证据测试完整用户旅程
    ├── 逐点验证规格合规性
    ├── 默认裁决：需要修改
    └── 只有在所有标准都有压倒性证据时才给出 READY
```

### 7.3 Phase 4 质量门控（最终门控）

**门控负责人**：Reality Checker（唯一权威）

| 标准 | 阈值 | 所需证据 |
|------|------|---------|
| 用户旅程完整 | 所有关键路径正常工作 | 端到端截图 |
| 跨设备一致性 | 桌面 + 平板 + 移动端 | 响应式截图 |
| 性能已认证 | P95 < 200ms，uptime > 99.9% | 负载测试结果 |
| 安全已验证 | 零严重漏洞 | 安全扫描报告 |
| 合规已认证 | 所有法规要求已满足 | Legal Compliance Checker 报告 |
| 规格合规 | 100% 规格要求 | 逐点验证 |

**裁决选项**：
- **READY** —— 继续发布（首次通过罕见）
- **NEEDS WORK** —— 返回 Phase 3 并附具体修复清单（预期）
- **NOT READY** —— 重大架构问题，返回 Phase 1/2

**预期**：首次实现通常需要 2-3 次修订循环。B/B+ 评分是正常和健康的。

---

## 8. Phase 5 —— 发布与增长

> **目标**：协调所有渠道的上市执行，同时进行。发布时产生最大影响。

### 8.1 活跃 Agent

| Agent | 阶段角色 | 主要输出 |
|-------|---------|---------|
| **Growth Hacker** | 发布战略负责人 | 增长 Playbook（含病毒循环） |
| **Content Creator** | 发布内容 | 博客文章、视频、社交内容 |
| **Social Media Strategist** | 跨平台活动 | 活动日历 + 内容 |
| **Twitter Engager** | Twitter/X 发布活动 | 线程策略 + 参与计划 |
| **TikTok Strategist** | TikTok 病毒内容 | 短视频策略 |
| **Instagram Curator** | 视觉发布活动 | 视觉内容 + Stories |
| **Reddit Community Builder** | 真实社区发布 | 社区参与计划 |
| **App Store Optimizer** | 商店优化（如移动端） | ASO 包 |
| **Executive Summary Generator** | 利益相关者沟通 | 发布执行摘要 |
| **Project Shepherd** | 发布协调 | 发布清单 + 时间线 |
| **DevOps Automator** | 部署执行 | 零停机部署 |
| **Infrastructure Maintainer** | 发布监控 | 实时仪表板 |

### 8.2 发布序列

```
T-7 天：预发布
├── Content Creator → 发布内容排队并安排
├── Social Media Strategist → 活动资产最终确定
├── Growth Hacker → 病毒机制测试并准备就绪
├── App Store Optimizer → 商店列表优化
├── DevOps Automator → 蓝绿部署准备
└── Infrastructure Maintainer → 自动扩缩容配置为 10 倍

T-0：发布日
├── DevOps Automator → 执行部署
├── Infrastructure Maintainer → 监控所有系统
├── Twitter Engager → 发布线程 + 实时参与
├── Reddit Community Builder → 真实社区帖子
├── Instagram Curator → 视觉发布内容
├── TikTok Strategist → 发布视频已发布
├── Support Responder → 客户支持激活
└── Analytics Reporter → 实时指标仪表板

T+1 到 T+7：发布后
├── Growth Hacker → 分析获客数据，优化漏斗
├── Feedback Synthesizer → 收集并分析早期用户反馈
├── Analytics Reporter → 每日指标报告
├── Content Creator → 基于反响的响应内容
├── Experiment Tracker → 启动 A/B 测试
└── Executive Summary Generator → 每日利益相关者简报
```

### 8.3 Phase 5 质量门控

**门控负责人**：Studio Producer + Analytics Reporter

| 标准 | 阈值 | 所需证据 |
|------|------|---------|
| 部署成功 | 零停机，所有健康检查通过 | DevOps 部署日志 |
| 系统稳定 | 前 48 小时无 P0/P1 事件 | 基础设施监控 |
| 用户获取激活 | 渠道正在引流 | Analytics Reporter 仪表板 |
| 反馈循环运行 | 用户反馈正在收集 | Feedback Synthesizer 报告 |
| 利益相关者已通知 | 执行摘要已交付 | Executive Summary Generator 输出 |

**输出**：稳定发布的产品及活跃增长渠道 → Phase 6 激活

---

## 9. Phase 6 —— 运营与演进

> **目标**：持续运营与改进。产品已上线 —— 现在让它茁壮成长。

### 9.1 活跃 Agent（持续）

| Agent | 节奏 | 职责 |
|-------|------|------|
| **Infrastructure Maintainer** | 持续 | 系统可靠性、uptime、性能 |
| **Support Responder** | 持续 | 客户支持和问题解决 |
| **Analytics Reporter** | 每周 | KPI 跟踪、仪表板、洞察 |
| **Feedback Synthesizer** | 双周 | 用户反馈分析和综合 |
| **Finance Tracker** | 每月 | 财务表现、预算跟踪 |
| **Legal Compliance Checker** | 每月 | 法规监控和合规 |
| **Trend Researcher** | 每月 | 市场情报和竞争分析 |
| **Executive Summary Generator** | 每月 | C-suite 报告 |
| **Sprint Prioritizer** | 每冲刺 | Backlog 梳理和冲刺规划 |
| **Experiment Tracker** | 每实验 | A/B 测试管理和分析 |
| **Growth Hacker** | 持续 | 获客优化和增长实验 |
| **Workflow Optimizer** | 每季度 | 流程改进和效率提升 |

### 9.2 持续改进循环

```
┌────────────────��─────────────────────────────────────────┐
│              持续改进循环                                 │
│                                                          │
│  衡量             分析            规划           行动     │
│  ┌─────────┐     ┌──────────┐     ┌─────────┐   ┌─────┐ │
│  │Analytics │────▶│Feedback  │────▶│Sprint   │──▶│构建│ │
│  │Reporter  │     │Synthesizer│    │Prioritizer│  │循环 │ │
│  └─────────┘     └──────────┘     └─────────┘   └─────┘ │
│       ▲                                            │      │
│       │              实验                          │      │
│       │              Tracker                       │      │
│       └────────────────────────────────────────────┘      │
│                                                          │
│  每月：Executive Summary Generator → C-suite 报告         │
│  每月：Finance Tracker → 财务表现                         │
│  每月：Legal Compliance Checker → 法规更新                │
│  每月：Trend Researcher → 市场情报                        │
│  每季度：Workflow Optimizer → 流程改进                    │
└──────────────────────────────────────────────────────────┘
```

---

## 10. Agent 协调矩阵

### 10.1 完整跨部门依赖图

此矩阵显示哪些 Agent 生产其他 Agent 消费的输出。阅读方式：**行 Agent 生产 → 列 Agent 消费**。

```
生产者 →          │ ENG │ DES │ MKT │ PRD │ PM  │ TST │ SUP │ SPC │ SPZ
────────────────────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼─────┼────
Engineering         │  ●  │     │     │     │     │  ●  │  ●  │  ●  │
Design              │  ●  │  ●  │  ●  │     │     │  ●  │     │  ●  │
Marketing           │     │     │  ●  │  ●  │     │     │  ●  │     │
Product             │  ●  │  ●  │  ●  │  ●  │  ●  │     │     │     │  ●
Project Management  │  ●  │  ●  │  ●  │  ●  │  ●  │  ●  │  ●  │  ●  │  ●
Testing             │  ●  │  ●  │     │  ●  │  ●  │  ●  │     │  ●  │
Support             │  ●  │     │  ●  │  ●  │  ●  │     │  ●  │     │  ●
Spatial Computing   │  ●  │  ●  │     │     │     │  ●  │     │  ●  │
Specialized         │  ●  │     │     │  ●  │  ●  │  ●  │  ●  │     │  ●

● = 活跃依赖（生产者创建此部门消费的工件）
```

### 10.2 关键交接对

这些是 NEXUS 中最高频的交接关系：

| 来源 | 目标 | 工件 | 频率 |
|------|------|------|------|
| Senior Project Manager | 所有开发者 | 任务列表 | 每冲刺 |
| UX Architect | Frontend Developer | CSS 设计系统 + 布局规范 | 每项目 |
| Backend Architect | Frontend Developer | API 规范 | 每功能 |
| Frontend Developer | Evidence Collector | 已实现功能 | 每任务 |
| Evidence Collector | Agents Orchestrator | QA 裁决（PASS/FAIL） | 每任务 |

| Agents Orchestrator | Developer（任意） | QA 反馈 + 重试指令 | 每次失败 |
| Brand Guardian | 所有设计 + 营销 | 品牌指南 | 每项目 |
| Analytics Reporter | Sprint Prioritizer | 表现数据 | 每冲刺 |
| Feedback Synthesizer | Sprint Prioritizer | 用户洞察 | 每冲刺 |
| Trend Researcher | Studio Producer | 市场情报 | 每月 |
| Reality Checker | Agents Orchestrator | 集成裁决 | 每阶段 |
| Executive Summary Generator | Studio Producer | 执行简报 | 每里程碑 |

---

## 11. 交接协议

### 11.1 标准交接模板

每次 Agent 间交接必须包含：

```markdown
## NEXUS 交接文档

### 元数据
- **来源**：[Agent 名称]（[部门]）
- **目标**：[Agent 名称]（[部门]）
- **阶段**：[当前 NEXUS 阶段]
- **任务引用**：[Sprint Prioritizer backlog 中的任务 ID]
- **优先级**：[关键 / 高 / 中 / 低]
- **时间戳**：[ISO 8601]

### 上下文
- **项目**：[项目名称及简要描述]
- **当前状态**：[到目前为止已完成的工作]
- **相关文件**：[要审查的文件/工件列表]
- **依赖**：[此工作依赖什么]

### 交付物请求
- **需要什么**：[具体、可衡量的交付物]
- **验收标准**：[如何衡量成功]
- **约束**：[技术、时间线或资源约束]
- **参考材料**：[链接到规格、设计、之前的工作]

### 质量期望
- **必须通过**：[具体质量标准]
- **所需证据**：[完成证明的样子]
- **交接给下一步**：[谁接收输出以及他们需要什么]
```

### 11.2 QA 反馈循环协议

当任务未通过 QA 时，反馈必须是可操作的：

```markdown
## QA 失败反馈

### 任务：[任务 ID 和描述]
### 尝试：[1/2/3]，最多 3 次
### 裁决：FAIL

### 发现的具体问题
1. **[问题类别]**：[带有截图引用的精确描述]
   - 预期：[应该发生什么]
   - 实际：[实际发生了什么]
   - 证据：[截图文件名或测试输出]

2. **[问题类别]**：[精确描述]
   - 预期：[...]
   - 实际：[...]
   - 证据：[...]

### 修复指令
- [具体、可操作的修复指令 1]
- [具体、可操作的修复指令 2]

### 要修改的文件
- [文件路径 1]：[需要改变什么]
- [文件路径 2]：[需要改变什么]

### 重试期望
- 修复上述问题并重新提交 QA
- 不要引入新功能 —— 只修复
- 尝试 [N+1] / 最多 3 次
```

### 11.3 升级协议

当任务超过 3 次重试尝试时：

```markdown
## 升级报告

### 任务：[任务 ID]
### 已耗尽尝试：3/3
### 升级级别：[到 Agents Orchestrator / 到 Studio Producer]

### 失败历史
- 尝试 1：[问题摘要和尝试的修复]
- 尝试 2：[问题摘要和尝试的修复]
- 尝试 3：[问题摘要和尝试的修复]

### 根本原因分析
- [为什么任务一直失败]
- [什么系统性问题阻碍了解决]

### 推荐解决方案
- [ ] 重新分配给不同的开发者 Agent
- [ ] 将任务分解为更小的子任务
- [ ] 修订架构/方法
- [ ] 接受当前状态及已知限制
- [ ] 推迟到未来冲刺

### 影响评估
- **阻塞**：[什么其他任务被此阻塞]
- **时间线影响**：[如何影响整体进度]
- **质量影响**：[存在什么质量妥协]
```

---

## 12. 质量门控

### 12.1 门控摘要

| 阶段 | 门控名称 | 门控负责人 | 通过标准 |
|------|---------|-----------|---------|
| 0 → 1 | 发现门控 | Executive Summary Generator | 市场已验证、用户需求已确认、法规路径清晰 |
| 1 → 2 | 架构门控 | Studio Producer + Reality Checker | 架构完整、品牌已定义、预算已批准、冲刺计划现实可行 |
| 2 → 3 | 基础门控 | DevOps Automator + Evidence Collector | CI/CD 工作、骨架应用运行、监控激活 |
| 3 → 4 | 功能门控 | Agents Orchestrator | 所有任务通过 QA、无严重 Bug、性能基线达标 |
| 4 → 5 | 生产门控 | Reality Checker（唯一权威） | 用户旅程完整、跨设备一致、安全已验证、规格合规 |
| 5 → 6 | 发布门控 | Studio Producer + Analytics Reporter | 部署成功、系统稳定、增长渠道激活 |

### 12.2 门控失败处理

```
IF 门控失败：
  ├── 门控负责人生成具体失败报告
  ├── Agents Orchestrator 将失败路由给负责 Agent
  ├── 失败项进入 Dev↔QA 循环（Phase 3 机制）
  ├── 最多 3 次门控重试后升级到 Studio Producer
  └── Studio Producer 决定：修复、降级范围、或接受风险
```

---

## 13. 风险管理

### 13.1 风险类别和负责人

| 风险类别 | 主要负责人 | 缓解 Agent | 升级路径 |
|---------|-----------|-----------|---------|
| 技术债务 | Backend Architect | Workflow Optimizer | Senior Developer |
| 安全漏洞 | Legal Compliance Checker | Infrastructure Maintainer | DevOps Automator |
| 性能退化 | Performance Benchmarker | Infrastructure Maintainer | Backend Architect |
| 品牌不一致 | Brand Guardian | UI Designer | Studio Producer |
| 范围蔓延 | Senior Project Manager | Sprint Prioritizer | Project Shepherd |
| 预算超支 | Finance Tracker | Studio Operations | Studio Producer |
| 法规不合规 | Legal Compliance Checker | Support Responder | Studio Producer |
| 市场变化 | Trend Researcher | Growth Hacker | Studio Producer |
| 团队瓶颈 | Project Shepherd | Studio Operations | Studio Producer |
| 质量回归 | Reality Checker | Evidence Collector | Agents Orchestrator |

### 13.2 风险响应矩阵

| 严重性 | 响应时间 | 决策权威 | 行动 |
|--------|---------|---------|------|
| **关键**（P0） | 立即 | Studio Producer | 全员，停止其他工作 |
| **高**（P1） | < 4 小时 | Project Shepherd | 专门 Agent 分配 |
| **中**（P2） | < 24 小时 | Agents Orchestrator | 下一冲刺优先级 |
| **低**（P3） | < 1 周 | Sprint Prioritizer | Backlog 项 |

---

## 14. 成功指标

### 14.1 流水线指标

| 指标 | 目标 | 测量 Agent |
|------|------|-----------|
| 阶段完成率 | 95% 首次通过 | Agents Orchestrator |
| 任务首次 QA 通过率 | 70%+ | Evidence Collector |
| 每任务平均重试次数 | < 1.5 | Agents Orchestrator |
| 流水线周期时间 | 冲刺估算 ±15% 内 | Project Shepherd |
| 质量门控通过率 | 80%+ 首次通过 | Reality Checker |

### 14.2 产品指标

| 指标 | 目标 | 测量 Agent |
|------|------|-----------|
| API 响应时间（P95） | < 200ms | Performance Benchmarker |
| 页面加载时间（LCP） | < 2.5s | Performance Benchmarker |
| 系统 uptime | > 99.9% | Infrastructure Maintainer |
| Lighthouse 分数 | > 90（性能 + 可访问性） | Frontend Developer |
| 安全漏洞 | 零严重 | Legal Compliance Checker |
| 规格合规 | 100% | Reality Checker |

### 14.3 业务指标

| 指标 | 目标 | 测量 Agent |
|------|------|-----------|
| 用户获取（MoM） | 20%+ 增长 | Growth Hacker |
| 激活率 | 60%+ 第一周 | Analytics Reporter |
| 留存（第 7 天 / 第 30 天） | 40% / 20% | Analytics Reporter |
| LTV:CAC 比率 | > 3:1 | Finance Tracker |
| NPS 分数 | > 50 | Feedback Synthesizer |
| 组合 ROI | > 25% | Studio Producer |

### 14.4 运营指标

| 指标 | 目标 | 测量 Agent |
|------|------|-----------|
| 部署频率 | 每天多次 | DevOps Automator |
| 平均恢复时间 | < 30 分钟 | Infrastructure Maintainer |
| 合规遵守 | 98%+ | Legal Compliance Checker |
| 利益相关者满意度 | 4.5/5 | Executive Summary Generator |
| 流程效率提升 | 每季度 20%+ | Workflow Optimizer |

---

## 15. 快速入门激活指南

### 15.1 NEXUS-Full 激活（企业）

```bash
# 步骤 1：初始化 NEXUS 流水线
"以 NEXUS-Full 模式为 [项目名称] 激活 Agents Orchestrator。
 项目规格：[规格文件路径]。
 执行完整的 7 阶段流水线及所有质量门控。"

# Orchestrator 将：
# 1. 读取项目规格
# 2. 激活 Phase 0 Agent 进行发现
# 3. 通过质量门控推进所有阶段
# 4. 自动管理 Dev↔QA 循环
# 5. 在每个阶段边界报告状态
```

### 15.2 NEXUS-Sprint 激活（功能/MVP）

```bash
# 步骤 1：初始化冲刺流水线
"以 NEXUS-Sprint 模式为 [功能/MVP 名称] 激活 Agents Orchestrator。
 需求：[简要描述或规格链接]。
 跳过 Phase 0（市场已验证）。
 从 Phase 1 开始进行架构和冲刺规划。"

# 推荐的 Agent 子集（15-25）：
# PM：Senior Project Manager、Sprint Prioritizer、Project Shepherd
# 设计：UX Architect、UI Designer、Brand Guardian
# 工程：Frontend Developer、Backend Architect、DevOps Automator
# + AI Engineer 或 Mobile App Builder（如适用）
# 测试：Evidence Collector、Reality Checker、API Tester、Performance Benchmarker
# 支持：Analytics Reporter、Infrastructure Maintainer
# 专项：Agents Orchestrator
```

### 15.3 NEXUS-Micro 激活（针对性任务）

```bash
# 步骤 1：直接 Agent 激活
"为 [任务描述] 激活 [特定 Agent]。
 上下文：[相关背景]。
 交付物：[预期的具体输出]。
 质量检查：Evidence Collector 完成后验证。"

# 常见的 NEXUS-Micro 配置：
#
# Bug 修复：
#   Backend Architect → API Tester → Evidence Collector
#
# 内容活动：
#   Content Creator → Social Media Strategist → Twitter Engager
#   + Instagram Curator + Reddit Community Builder
#
# 性能问题：
#   Performance Benchmarker → Infrastructure Maintainer → DevOps Automator
#
# 合规审计：
#   Legal Compliance Checker → Executive Summary Generator
#
# 市场研究：
#   Trend Researcher → Analytics Reporter → Executive Summary Generator
#
# UX 改进：
#   UX Researcher → UX Architect → Frontend Developer → Evidence Collector
```

### 15.4 Agent 激活提示模板

#### 编排器（流水线启动）
```
你是为 [项目] 运行 NEXUS 流水线的 Agents Orchestrator。

项目规格：[路径]
模式：[Full/Sprint/Micro]
当前阶段：[阶段 N]

执行 NEXUS 协议：
1. 读取项目规格
2. 按 NEXUS 策略激活��段 [N] Agent
3. 使用 NEXUS 交接模板管理交接
4. 在阶段推进前强制质量门控
5. 跟踪所有任务及状态报告
6. 对所有实现任务运行 Dev↔QA 循环
7. 每个任务 3 次失败尝试后升级

报告格式：NEXUS 流水线状态报告（见策略文档中的模板）
```

#### 开发者 Agent（任务实现）
```
你是 [Agent 名称]，在 NEXUS 流水线内工作。

阶段：[当前阶段]
任务：[Sprint Prioritizer backlog 中的任务 ID 和描述]
架构参考：[架构文档路径]
设计系统：[CSS/设计令牌路径]
品牌指南：[品牌文档路径]

按以下要求实现此任务：
1. 精确遵循架构规范
2. 遵循设计系统令牌和模式
3. 遵循品牌指南以确保视觉一致性
4. 可访问性标准（WCAG 2.1 AA）

完成后，你的工作将由 Evidence Collector 审查。
验收标准：[任务列表中的具体标准]
```

#### QA Agent（任务验证）
```
你是 [QA Agent]，在 NEXUS 流水线内验证工作。

阶段：[当前阶段]
任务：[任务 ID 和描述]
开发者：[哪个 Agent 实现了此任务]
尝试：[N] / 最多 3 次

验证以下内容：
1. 任务验收标准：[具体标准]
2. 架构规范：[路径]
3. 品牌指南：[路径]
4. 性能要求：[具体阈值]

提供裁决：PASS 或 FAIL
如果 FAIL：包含具体问题、证据和修复指令
使用 NEXUS QA 反馈循环协议格式
```

---

## 附录 A：部门快速参考

### Engineering 部门 —— "正确构建"
| Agent | 超能力 | 激活触发 |
|-------|--------|---------|
| Frontend Developer | React/Vue/Angular、Core Web Vitals、可访问性 | 任何 UI 实现任务 |
| Backend Architect | 可扩展系统、数据库设计、API 架构 | 服务端架构或 API 工作 |
| Mobile App Builder | iOS/Android、React Native、Flutter | 移动应用开发 |
| AI Engineer | ML 模型、LLM、RAG 系统、数据流水线 | 任何 AI/ML 功能 |
| DevOps Automator | CI/CD、IaC、Kubernetes、监控 | 基础设施或部署工作 |
| Rapid Prototyper | Next.js、Supabase、3 天 MVP | 快速验证或概念验证 |
| Senior Developer | Laravel/Livewire、高级实现 | 复杂或高级功能工作 |

### Design 部门 —— "美化构建"
| Agent | 超能力 | 激活触发 |
|-------|--------|---------|
| UI Designer | 视觉设计系统、组件库 | 界面设计或组件创建 |
| UX Researcher | 用户测试、行为分析、用户画像 | 用户研究或可用性测试 |
| UX Architect | CSS 系统、布局框架、技术 UX | 技术基础或架构 |
| Brand Guardian | 品牌标识、一致性、定位 | 品牌战略或一致性审计 |
| Visual Storyteller | 视觉叙事、多媒体内容 | 视觉内容或叙事需求 |
| Whimsy Injector | 微交互、愉悦感、个性 | 为 UX 添加乐趣和个性 |
| Image Prompt Engineer | AI 图像生成提示、摄影 | AI 工具的摄影提示创建 |

### Marketing 部门 —— "快速增长"
| Agent | 超能力 | 激活触发 |
|-------|--------|---------|
| Growth Hacker | 病毒循环、漏斗优化、实验 | 用户获取或增长战略 |
| Content Creator | 多平台内容、编辑日历 | 内容战略或创建 |
| Twitter Engager | 实时参与、思想领导力 | Twitter/X 活动 |
| TikTok Strategist | 病毒短视频、算法优化 | TikTok 增长战略 |
| Instagram Curator | 视觉叙事、美学开发 | Instagram 活动 |
| Reddit Community Builder | 真实参与、价值驱动内容 | Reddit 社区战略 |
| App Store Optimizer | ASO、转化优化 | 移动应用商店存在 |
| Social Media Strategist | 跨平台战略、活动 | 多平台社交活动 |

### Product 部门 —— "构建正确的东西"
| Agent | 超能力 | 激活触发 |
|-------|--------|---------|
| Sprint Prioritizer | RICE 评分、敏捷规划、速度 | 冲刺规划或 Backlog 梳理 |
| Trend Researcher | 市场情报、竞争分析 | 市场研究或机会评估 |
| Feedback Synthesizer | 用户反馈分析、情感分析 | 用户反馈处理 |

### Project Management 部门 —— "保持在轨道上"
| Agent | 超能力 | 激活触发 |
|-------|--------|---------|
| Studio Producer | 组合战略、执行编排 | 战略规划或组合管理 |
| Project Shepherd | 跨职能协调、利益相关者对齐 | 复杂项目协调 |
| Studio Operations | 日常效率、流程优化 | 运营支持 |
| Experiment Tracker | A/B 测试、假设验证 | 实验管理 |
| Senior Project Manager | 规格转任务、现实范围界定 | 任务规划或范围管理 |

### Testing 部门 —— "证明它能工作"
| Agent | 超能力 | 激活触发 |
|-------|--------|---------|
| Evidence Collector | 基于截图的 QA、视觉证明 | 任何视觉验证需求 |
| Reality Checker | 基于证据的认证、怀疑性评估 | 最终集成测试 |
| Test Results Analyzer | 测试评估、质量指标 | 测试输出分析 |
| Performance Benchmarker | 负载测试、性能优化 | 性能测试 |
| API Tester | API 验证、集成测试 | API 端点测试 |
| Tool Evaluator | 技术评估、工具选择 | 技术评估 |
| Workflow Optimizer | 流程分析、效率改进 | 流程优化 |

### Support 部门 —— "维持运行"
| Agent | 超能力 | 激活触发 |
|-------|--------|---------|
| Support Responder | 客户服务、问题解决 | 客户支持需求 |
| Analytics Reporter | 数据分析、仪表板、KPI 跟踪 | 商业智能或报告 |
| Finance Tracker | 财务规划、预算管理 | 财务分析或预算 |
| Infrastructure Maintainer | 系统可靠性、性能优化 | 基础设施管理 |
| Legal Compliance Checker | 合规、法规、法律审查 | 法律或合规需求 |
| Executive Summary Generator | C-suite 沟通、SCQA 框架 | 执行报告 |

### Spatial Computing 部门 —— "让他们沉浸"
| Agent | 超能力 | 激活触发 |
|-------|--------|---------|
| XR Interface Architect | 空间交互设计 | AR/VR/XR 界面设计 |
| macOS Spatial/Metal Engineer | Swift、Metal、高性能 3D | macOS 空间计算 |
| XR Immersive Developer | WebXR、基于浏览器的 AR/VR | 基于浏览器的沉浸式体验 |
| XR Cockpit Interaction Specialist | 驾驶舱式控制 | 沉浸式控制界面 |
| visionOS Spatial Engineer | Apple Vision Pro 开发 | Vision Pro 应用 |
| Terminal Integration Specialist | CLI 工具、终端工作流 | 开发者工具集成 |

### Specialized 部门 —— "连接一切"
| Agent | 超能力 | 激活触发 |
|-------|--------|---------|
| Agents Orchestrator | 多 Agent 流水线管理 | 任何多 Agent 工作流 |
| Data Analytics Reporter | 商业智能、深度分析 | 深度数据分析 |
| LSP/Index Engineer | Language Server Protocol、代码智能 | 代码智能系统 |
| Sales Data Extraction Agent | Excel 监控、销售指标提取 | 销售数据获取 |
| Data Consolidation Agent | 销售数据聚合、仪表板报告 | 区域和代表报告 |
| Report Distribution Agent | 自动报告分发 | 定时报告分发 |

---

## 附录 B：NEXUS 流水线状态报告模板

```markdown
# NEXUS 流水线状态报告

## 流水线元数据
- **项目**：[名称]
- **模式**：[Full / Sprint / Micro]
- **当前阶段**：[0-6]
- **开始时间**：[时间戳]
- **预计完成**：[时间戳]

## 阶段进度
| 阶段 | 状态 | 完成度 | 门控结果 |
|------|------|--------|---------|
| 0 - 发现 | ✅ 完成 | 100% | PASSED |
| 1 - 战略 | ✅ 完成 | 100% | PASSED |
| 2 - 基础 | 🔄 进行中 | 75% | PENDING |
| 3 - 构建 | ⏳ 待定 | 0% | — |
| 4 - 加固 | ⏳ 待定 | 0% | — |
| 5 - 发布 | ⏳ 待定 | 0% | — |
| 6 - 运营 | ⏳ 待定 | 0% | — |

## 当前阶段详情
**阶段**：[N] - [名称]
**活跃 Agent**：[列表]
**任务**：[已完成/总数]
**当前任务**：[ID] - [描述]
**QA 状态**：[PASS/FAIL/IN_PROGRESS]
**重试次数**：[N/3]

## 质量指标
- 首次通过任务：[X/Y]（[Z]%）
- 每任务平均重试：[N]
- 发现的严重问题：[计数]
- 已解决的严重问题：[计数]

## 风险登记
| 风险 | 严重性 | 状态 | 负责人 |
|------|--------|------|-------|
| [描述] | [P0-P3] | [活跃/已缓解/已关闭] | [Agent] |

## 下一步行动
1. [立即下一步]
2. [后续步骤]
3. [即将到来的里程碑]

---
**报告生成时间**：[时间戳]
**Orchestrator**：Agents Orchestrator
**流水线健康状态**：[ON_TRACK / AT_RISK / BLOCKED]
```

---

## 附录 C：NEXUS 术语表

| 术语 | 定义 |
|------|------|
| **NEXUS** | Network of EXperts, Unified in Strategy（专家网络，战略统一） |
| **质量门控（Quality Gate）** | 阶段之间需要基于证据审批的强制检查点 |
| **Dev↔QA 循环** | 持续的开发-测试循环，每个任务必须通过 QA 才能继续 |
| **交接（Handoff）** | Agent 之间工作和上下文的结构化转移 |
| **门控负责人（Gate Keeper）** | 有权批准或拒绝阶段推进的 Agent |
| **升级（Escalation）** | 重试次数用尽后将阻塞任务路由给更高级别权威 |
| **NEXUS-Full** | 所有 Agent 的完整流水线激活 |
| **NEXUS-Sprint** | 15-25 个 Agent 的专注流水线，用于功能/MVP 工作 |
| **NEXUS-Micro** | 5-10 个 Agent 的针对性激活，用于特定任务 |
| **流水线完整性（Pipeline Integrity）** | 没有通过质量门控任何阶段都不能推进的原则 |
| **上下文连续性（Context Continuity）** | 每次交接都携带完整上下文的原则 |
| **证据胜于声明（Evidence Over Claims）** | 质量评估需要证明而非断言的原则 |

---

<div align="center">

**🌐 NEXUS：9 个部门。7 个阶段。一个统一的战略。🌐**

*从发现到持续运营 —— 每个 Agent 都知道自己的角色、时机和交接。*

</div>