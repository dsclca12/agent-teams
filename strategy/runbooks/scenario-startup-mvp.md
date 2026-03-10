# 🚀 Runbook：Startup MVP 构建

> **模式**：NEXUS-Sprint | **持续时间**：4-6 周 | **Agent 数量**：18-22

---

## 场景

您正在构建一个 Startup MVP —— 一个需要快速验证产品市场契合度的新产品。速度很重要，但质量也很重要。您需要在 4-6 周内从想法到上线产品及真实用户。

## Agent 名册

### 核心团队（始终激活）
| Agent | 角色 |
|-------|------|
| Agents Orchestrator | 流水线控制器 |
| Senior Project Manager | 规格转任务 |
| Sprint Prioritizer | Backlog 管理 |
| UX Architect | 技术基础 |
| Frontend Developer | UI 实现 |
| Backend Architect | API 和数据库 |
| DevOps Automator | CI/CD 和部署 |
| Evidence Collector | 每个任务的 QA |
| Reality Checker | 最终质量门控 |

### 增长团队（第 3 周起激活）
| Agent | 角色 |
|-------|------|
| Growth Hacker | 获客策略 |
| Content Creator | 发布内容 |
| Social Media Strategist | 社交活动 |

### 支持团队（按需）
| Agent | 角色 |
|-------|------|
| Brand Guardian | 品牌标识 |
| Analytics Reporter | 指标和仪表板 |
| Rapid Prototyper | 快速验证实验 |
| AI Engineer | 如产品包含 AI 功能 |
| Performance Benchmarker | 发布前负载测试 |
| Infrastructure Maintainer | 生产设置 |

## 周执行计划

### 第 1 周：发现 + 架构（压缩的 Phase 0 + Phase 1）

```
第 1-2 天：压缩发现
├── Trend Researcher → 快速竞争扫描（1 天，非完整报告）
├── UX Architect → 关键用户流程线框图
└── Senior Project Manager → 将规格转换为任务列表

第 3-4 天：架构
├── UX Architect → CSS 设计系统 + 组件架构
├── Backend Architect → 系统架构 + 数据库 Schema
├── Brand Guardian → 快速品牌基础（颜色、排版、语调）
└── Sprint Prioritizer → RICE 评分的 Backlog + 冲刺计划

第 5 天：基础设置
├── DevOps Automator → CI/CD 流水线 + 环境
├── Frontend Developer → 项目脚手架
├── Backend Architect → 数据库 + API 脚手架
└── 质量门控：架构包已批准
```

### 第 2-3 周：核心构建（Phase 2 + Phase 3）

```
冲刺 1（第 2 周）：
├── Agents Orchestrator 管理 Dev↔QA 循环
├── Frontend Developer → 核心 UI（认证、主视图、导航）
├── Backend Architect → 核心 API（认证、CRUD、业务逻辑）
├── Evidence Collector → 每个已完成任务的 QA
├── AI Engineer → 如适用的 ML 功能
└── 周末冲刺评审

冲刺 2（第 3 周）：
├── 继续 Dev↔QA 循环完成剩余功能
├── Growth Hacker → 设计病毒机制 + 推荐系统
├── Content Creator → 开始发布内容创建
├── Analytics Reporter → 设置跟踪和仪表板
└── 周末冲刺评审
```

### 第 4 周：打磨 + 加固（Phase 4）

```
第 1-2 天：质量冲刺
├── Evidence Collector → 完整截图套件
├── Performance Benchmarker → 负载测试
├── Frontend Developer → 修复 QA 问题
├── Backend Architect → 修复 API 问题
└── Brand Guardian → 品牌一致性审计

第 3-4 天：现实检查
├── Reality Checker → 最终集成测试
├── Infrastructure Maintainer → 生产就绪
└── DevOps Automator → 生产部署准备

第 5 天：门控决策
├── Reality Checker 裁决
├── IF 需要修改：快速修复循环（2-3 天）
├── IF 就绪：继续发布
└── Executive Summary Generator → 利益相关者简报
```

### 第 5-6 周：发布 + 增长（Phase 5）

```
第 5 周：发布
├── DevOps Automator → 生产部署
├── Growth Hacker → 激活获客渠道
├── Content Creator → 发布发布内容
├── Social Media Strategist → 跨平台活动
├── Analytics Reporter → 实时监控
└── Support Responder → 用户支持激活

第 6 周：优化
├── Growth Hacker → 分析并优化渠道
├── Feedback Synthesizer → 收集早期用户反馈
├── Experiment Tracker → 启动 A/B 测试
├── Analytics Reporter → 第 1 周分析
└── Sprint Prioritizer → 规划迭代冲刺
```

## 关键决策

| 决策点 | 何时 | 谁决定 |
|-------|------|-------|
| 概念 Go/No-Go | 第 2 天结束 | Studio Producer |
| 架构批准 | 第 4 天结束 | Senior Project Manager |
| MVP 功能范围 | 冲刺规划 | Sprint Prioritizer |
| 生产就绪 | 第 4 周第 5 天 | Reality Checker |
| 发布时机 | Reality Checker READY 后 | Studio Producer |

## 成功标准

| 指标 | 目标 |
|------|------|
| 上线产品时间 | ≤ 6 周 |
| 核心功能完成 | 100% MVP 范围 |
| 首批用户入驻 | 发布后 48 小时内 |
| 系统 uptime | 第一周 > 99% |
| 收集用户反馈 | 前 2 周内 ≥ 50 条回复 |

## 常见陷阱与缓解措施

| 陷阱 | 缓解措施 |
|------|---------|
| 构建过程中的范围蔓延 | Sprint Prioritizer 执行 MoSCoW —— "不会做"就是不会做 |
| 过度工程化以扩展规模 | Rapid Prototyper 心态 —— 先验证，后扩展 |
| 为速度跳过 QA | Evidence Collector 对每个任务运行 —— 无例外 |
| 没有监控就发布 | Infrastructure Maintainer 在第 1 周设置监控 |
| 没有反馈机制 | 分析 + 反馈收集内置到冲刺 1 |