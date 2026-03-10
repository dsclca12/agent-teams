# 🚨 Runbook：事件响应

> **模式**：NEXUS-Micro | **持续时间**：分钟到小时 | **Agent 数量**：3-8

---

## 场景

生产环境中出现问题。用户受到影响。响应速度很重要，但正确处理也很重要。本 Runbook 涵盖从检测到事后分析的全过程。

## 严重性分类

| 级别 | 定义 | 示例 | 响应时间 |
|------|------|------|---------|
| **P0 —— 关键** | 服务完全中断、数据丢失、安全漏洞 | 数据库损坏、DDoS 攻击、认证系统故障 | 立即（全员） |
| **P1 —— 高** | 主要功能损坏、显著性能退化 | 支付处理中断、50%+ 错误率、10 倍延迟 | < 1 小时 |
| **P2 —— 中** | 次要功能损坏、有变通方案可用 | 搜索不工作、非关键 API 错误 | < 4 小时 |
| **P3 —— 低** | 外观问题、轻微不便 | 样式 Bug、错别字、轻微 UI 故障 | 下个冲刺 |

## 按严重性的响应团队

### P0 —— 关键响应团队
| Agent | 角色 | 行动 |
|-------|------|------|
| **Infrastructure Maintainer** | 事件指挥官 | 评估范围、协调响应 |
| **DevOps Automator** | 部署/回滚 | 如需要执行回滚 |
| **Backend Architect** | 根本原因调查 | 诊断系统问题 |
| **Frontend Developer** | UI 端调查 | 诊断客户端问题 |
| **Support Responder** | 用户沟通 | 状态页更新、用户通知 |
| **Executive Summary Generator** | 利益相关者沟通 | 实时执行更新 |

### P1 —— 高响应团队
| Agent | 角色 |
|-------|------|
| **Infrastructure Maintainer** | 事件指挥官 |
| **DevOps Automator** | 部署支持 |
| **相关开发者 Agent** | 修复实现 |
| **Support Responder** | 用户沟通 |

### P2 —— 中响应
| Agent | 角色 |
|-------|------|
| **相关开发者 Agent** | 修复实现 |
| **Evidence Collector** | 验证修复 |

### P3 —— 低响应
| Agent | 角色 |
|-------|------|
| **Sprint Prioritizer** | 添加到 Backlog |

## 事件响应序列

### 步骤 1：检测与分类（0-5 分钟）

```
触发：来自监控的告警 / 用户报告 / Agent 检测

Infrastructure Maintainer：
1. 确认告警
2. 评估范围和影响
   - 多少用户受影响？
   - 哪些服务受影响？
   - 数据是否有风险？
3. 分类严重性（P0/P1/P2/P3）
4. 激活适当的响应团队
5. 创建事件频道/线程

输出：事件分类 + 响应团队激活
```

### 步骤 2：调查（5-30 分钟）

```
并行调查：

Infrastructure Maintainer：
├── 检查系统指标（CPU、内存、网络、磁盘）
├── 审查错误日志
├── 检查最近部署
└── 验证外部依赖

Backend Architect（如 P0/P1）：
├── 检查数据库健康
├── 审查 API 错误率
├── 检查服务通信
└── 识别故障组件

DevOps Automator：
├── 审查最近部署历史
├── 检查 CI/CD 流水线状态
├── 如需要准备回滚
└── 验证基础设施状态

输出：根本原因识别（或缩小到组件）
```

### 步骤 3：缓解（15-60 分钟）

```
决策树：

IF 由最近部署引起：
  → DevOps Automator：执行回滚
  → Infrastructure Maintainer：验证恢复
  → Evidence Collector：确认修复

IF 由基础设施问题引起：
  → Infrastructure Maintainer：扩缩容/重启/故障转移
  → DevOps Automator：支持基础设施变更
  → 验证恢复

IF 由代码 Bug 引起：
  → 相关开发者 Agent：实现热修复
  → Evidence Collector：验证修复
  → DevOps Automator：部署热修复
  → Infrastructure Maintainer：监控恢复

IF 由外部依���引起：
  → Infrastructure Maintainer：激活回退/缓存
  → Support Responder：向用户沟通
  → 监控外部恢复

整个过程中：
  → Support Responder：每 15 分钟更新状态页
  → Executive Summary Generator：简报利益相关者（仅 P0）
```

### 步骤 4：解决验证（修复后）

```
Evidence Collector：
1. 验证修复解决了问题
2. 工作状态的截图证据
3. 确认没有引入新问题

Infrastructure Maintainer：
1. 验证所有指标恢复正常
2. 确认没有级联故障
3. 修复后监控 30 分钟

API Tester（如 API 相关）：
1. 对受影响端点运行回归
2. 验证响应时间正常化
3. 确认错误率回到基线

输出：事件解决确认
```

### 步骤 5：事后分析（48 小时内）

```
Workflow Optimizer 主持事后分析：

1. 时间线重建
   - 问题何时引入？
   - 何时被检测到？
   - 何时解决？
   - 总用户影响持续时间

2. 根本原因分析
   - 什么失败了？
   - 为什么失败？
   - 为什么没有更早发现？
   - 5 个为什么分析

3. 影响评估
   - 受影响用户
   - 收入影响
   - 声誉影响
   - 数据影响

4. 预防措施
   - 什么监控能更早发现这个问题？
   - 什么测试能防止这个问题？
   - 需要什么流程变更？
   - 需要什么基础设施变更？

5. 行动项
   - [行动] → [负责人] → [截止日期]
   - [行动] → [负责人] → [截止日期]
   - [行动] → [负责人] → [截止日期]

输出：事后分析报告 → Sprint Prioritizer 将预防任务添加到 Backlog
```

## 沟通模板

### 状态页更新（Support Responder）
```
[时间戳] — [服务名称] 事件

状态：[调查中 / 已识别 / 监控中 / 已解决]
影响：[用户影响描述]
当前行动：[我们正在做什么]
下次更新：[预期下次更新的时间]
```

### 执行更新（Executive Summary Generator —— 仅 P0）
```
事件简报 — [时间戳]

情况：[服务] [中断/退化]，影响 [N 用户/% 流量]
原因：[已知/调查中] — [如已知则简要描述]
行动：[正在做什么] — 预计 [时间估算]
影响：[业务影响 — 收入、用户、声誉]
下次更新：[时间戳]
```

## 升级矩阵

| 条件 | 升级给 | 行动 |
|------|-------|------|
| P0 30 分钟内未解决 | Studio Producer | 额外资源、供应商升级 |
| P1 2 小时内未解决 | Project Shepherd | 资源重新分配 |
| 怀疑数据泄露 | Legal Compliance Checker | 法规通知评估 |
| 用户数据受影响 | Legal Compliance Checker + Executive Summary Generator | GDPR/CCPA 通知 |
| 收入影响 > $X | Finance Tracker + Studio Producer | 业务影响评估 |