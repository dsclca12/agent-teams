# 🔨 Phase 3 Playbook —— 构建与迭代

> **持续时间**：2-12 周（视范围而定）| **Agent 数量**：15-30+ | **门控负责人**：Agents Orchestrator

---

## 目标

通过持续的 Dev↔QA 循环实现所有功能。每个任务在下一个任务开始前都要验证。这是大部分工作发生的地方 —— 也是 NEXUS 编排发挥最大价值的地方。

## 前置条件

- [ ] Phase 2 质量门控通过（基础已验证）
- [ ] Sprint Prioritizer Backlog 可用及 RICE 分数
- [ ] CI/CD 流水线可操作
- [ ] 设计系统和组件库就绪
- [ ] API 脚手架及认证系统就绪

## Dev↔QA 循环 —— 核心机制

Agents Orchestrator 通过此循环管理每个任务：

```
FOR EACH 任务 IN 冲刺_backlog（按 RICE 分数排序）：

  1. ASSIGN 任务给适当的开发者 Agent（见分配矩阵）
  2. Developer IMPLEMENTS 任务
  3. Evidence Collector TESTS 任务
     - 视觉截图（桌面、平板、移动端）
     - 针对验收标准的功能验证
     - 品牌一致性检查
  4. IF 裁决 == PASS：
       标记任务完成
       移至下一个任务
     ELIF 裁决 == FAIL AND 尝试 < 3：
       将 QA 反馈发送给开发者
       Developer FIXES 具体问题
       返回步骤 3
     ELIF 尝试 >= 3：
       ESCALATE 给 Agents Orchestrator
       Orchestrator 决定：重新分配、分解、推迟或接受
  5. UPDATE 流水线状态报告
```

## Agent 分配矩阵

### 主要开发者分配

| 任务类别 | 主要 Agent | 备用 Agent | QA Agent |
|---------|-----------|-----------|----------|
| **React/Vue/Angular UI** | Frontend Developer | Rapid Prototyper | Evidence Collector |
| **REST/GraphQL API** | Backend Architect | Senior Developer | API Tester |
| **数据库操作** | Backend Architect | — | API Tester |
| **移动端（iOS/Android）** | Mobile App Builder | — | Evidence Collector |
| **ML 模型/流水线** | AI Engineer | — | Test Results Analyzer |
| **CI/CD/基础设施** | DevOps Automator | Infrastructure Maintainer | Performance Benchmarker |
| **高级/复杂功能** | Senior Developer | Backend Architect | Evidence Collector |
| **快速原型/POC** | Rapid Prototyper | Frontend Developer | Evidence Collector |
| **WebXR/沉浸式** | XR Immersive Developer | — | Evidence Collector |
| **visionOS** | visionOS Spatial Engineer | macOS Spatial/Metal Engineer | Evidence Collector |
| **驾驶舱控制** | XR Cockpit Interaction Specialist | XR Interface Architect | Evidence Collector |
| **CLI/终端工具** | Terminal Integration Specialist | — | API Tester |
| **代码智能** | LSP/Index Engineer | — | Test Results Analyzer |
| **性能优化** | Performance Benchmarker | Infrastructure Maintainer | Performance Benchmarker |

### 专家支持（按需激活）

| 专家 | 何时激活 | 触发条件 |
|------|---------|---------|
| UI Designer | 组件需要视觉优化 | 开发者请求设计指导 |
| Whimsy Injector | 功能需要愉悦感/个性 | UX 审查发现机会 |
| Visual Storyteller | 需要视觉叙事内容 | 内容需要视觉资产 |
| Brand Guardian | 品牌一致性关注 | QA 发现品牌偏差 |
| XR Interface Architect | 需要空间交互设计 | XR 功能需要 UX 指导 |
| Data Analytics Reporter | 需要深度数据分析 | 功能需要分析集成 |

## 并行构建轨道

对于 NEXUS-Full 部署，四条轨道同时运行：

### 轨道 A：核心产品开发
```
管理：Agents Orchestrator（Dev↔QA 循环）
Agent：Frontend Developer、Backend Architect、AI Engineer、
        Mobile App Builder、Senior Developer
QA：Evidence Collector、API Tester、Test Results Analyzer

冲刺节奏：2 周冲刺
每日：任务实现 + QA 验证
冲刺结束：冲刺评审 + 回顾
```

### 轨道 B：增长与营销准备
```
管理：Project Shepherd
Agent：Growth Hacker、Content Creator、Social Media Strategist、
        App Store Optimizer

冲刺节奏：与轨道 A 里程碑对齐
活动：
- Growth Hacker → 设计病毒循环和推荐机制
- Content Creator → 构建发布内容流水线
- Social Media Strategist → 规划跨平台活动
- App Store Optimizer → 准备商店列表（如移动端）
```

### 轨道 C：质量与运营
```
管理：Agents Orchestrator
Agent：Evidence Collector、API Tester、Performance Benchmarker、
        Workflow Optimizer、Experiment Tracker

持续活动：
- Evidence Collector → 每个任务的截图 QA
- API Tester → 每个 API 任务的端点验证
- Performance Benchmarker → 定期负载测试
- Workflow Optimizer → 流程改进识别
- Experiment Tracker → 已验证功能的 A/B 测试设置
```

### 轨道 D：品牌与体验打磨
```
管理：Brand Guardian
Agent：UI Designer、Brand Guardian、Visual Storyteller、
        Whimsy Injector

触发活动：
- UI Designer → QA 发现视觉问题时的组件优化
- Brand Guardian → 定期品牌一致性审计
- Visual Storyteller → 功能完成时的视觉叙事资产
- Whimsy Injector → 微交互和愉悦时刻
```

## 冲刺执行模板

### 冲刺规划（第 1 天）

```
Sprint Prioritizer 激活：
1. 用更新的 RICE 分数审查 Backlog
2. 根据团队速度选择冲刺任务
3. 将任务分配给开发者 Agent
4. 识别依赖和排序
5. 设定冲刺目标和成功标准

输出：带任务分配的冲刺计划
```

### 每日执行（第 2 天到第 N-1 天）

```
Agents Orchestrator 管理：
1. 当前任务状态检查
2. Dev↔QA 循环执行
3. 阻塞因素识别和解决
4. 进度跟踪和报告

状态报告格式：
- 今日完成任务：[列表]
- QA 中的任务：[列表]
- 开发中的任务：[列表]
- 阻塞的任务：[列表及原因]
- QA 通过率：[X/Y]
```

### 冲刺评审（第 N 天）

```
Project Shepherd 主持：
1. 演示已完成功能
2. 审查每个任务的 QA 证据
3. 收集利益相关者反馈
4. 根据学习更新 Backlog

参与者：所有活跃 Agent + 利益相关者
输出：冲刺评审摘要
```

### 冲刺回顾

```
Workflow Optimizer 主持：
1. 哪些做得好？
2. 哪些可以改进？
3. 下个冲刺我们将改变什么？
4. 流程效率指标

输出：回顾行动项
```

## Orchestrator 决策逻辑

### 任务失败处理

```
WHEN 任务未通过 QA：
  IF 尝试 == 1：
    → 将具体 QA 反馈发送给开发者
    → Developer 只修复已识别的问题
    → 重新提交 QA
    
  IF 尝试 == 2：
    → 发送累积的 QA 反馈
    → 考虑：开发者 Agent 是否合适？
    → Developer 在额外上下文下修复
    → 重新提交 QA
    
  IF 尝试 == 3：
    → ESCALATE
    → 选项：
      a) 重新分配给不同的开发者 Agent
      b) 将任务分解为更小的子任务
      c) 修订方法/架构
      d) 接受已知限制（文档化）
      e) 推迟到未来冲刺
    → 文档化决策和理由
```

### 并行任务管理

```
WHEN 多个任务没有依赖：
  → 同时分配给不同的开发者 Agent
  → 每个运行独立的 Dev↔QA 循环
  → Orchestrator 并发跟踪所有循环
  → 按依赖顺序合并已完成的任务

WHEN 任务有依赖：
  → 等待依赖通过 QA
  → 然后分配依赖任务
  → 在交接中包含依赖上下文
```

## 质量门控检查清单

| # | 标准 | 证据来源 | 状态 |
|---|------|---------|------|
| 1 | 所有冲刺任务通过 QA（100% 完成） | Evidence Collector 每任务截图 | ��� |
| 2 | 所有 API 端点已验证 | API Tester 回归报告 | ☐ |
| 3 | 性能基线达标（P95 < 200ms） | Performance Benchmarker 报告 | ☐ |
| 4 | 品牌一致性已验证（95%+ 符合度） | Brand Guardian 审计 | ☐ |
| 5 | 无严重 Bug（零 P0/P1 未解决） | Test Results Analyzer 摘要 | ☐ |
| 6 | 所有验收标准已满足 | 逐任务验证 | ☐ |
| 7 | 所有 PR 已完成代码审查 | Git 历史证据 | ☐ |

## 门控决策

**门控负责人**：Agents Orchestrator

- **PASS**：功能完整的应用 → Phase 4 激活
- **CONTINUE**：需要更多冲刺 → 继续 Phase 3
- **ESCALATE**：系统性问题 → Studio Producer 介入

## 交接到 Phase 4

```markdown
## Phase 3 → Phase 4 交接包

### 给 Reality Checker：
- 完整应用（所有功能已实现）
- Dev↔QA 循环的所有 QA 证据
- API Tester 回归结果
- Performance Benchmarker 基线数据
- Brand Guardian 一致性审计
- 已知问题列表（如有接受的限制）

### 给 Legal Compliance Checker：
- 数据处理实现详情
- 隐私政策实现
- 同意管理实现
- 已实施的安全措施

### 给 Performance Benchmarker：
- 负载测试的应用 URL
- 预期流量模式
- 来自架构的性能预算

### 给 Infrastructure Maintainer：
- 生产环境要求
- 扩缩容配置需求
- 监控告警阈值
```

---

*当所有冲刺任务通过 QA、所有 API 端点已验证、性能基线达标、无严重 Bug 未解决时，Phase 3 完成。*