# Nexus Spatial：完整 Agency 发现实践

> **实践类型：** 多 agent 产品发现
> **日期：** 2026年3月5日
> **部署的 Agents：** 8 个（并行）
> **持续时间：** 约 10 分钟实际时间
> **目的：** 展示从机会识别到全面规划的全 agency 编排能力

---

## 目录

1. [机会发现](#1-机会发现)
2. [市场验证](#2-市场验证)
3. [技术架构](#3-技术架构)
4. [品牌策略](#4-品牌策略)
5. [Go-to-Market 与增长](#5-go-to-market-与增长)
6. [客户支持蓝图](#6-客户支持蓝图)
7. [UX 研究与设计方向](#7-ux-研究与设计方向)
8. [项目执行计划](#8-项目执行计划)
9. [空间界面架构](#9-空间界面架构)
10. [跨 Agent 综合](#10-跨-agent-综合)

---

## 1. 机会发现

### 如何发现的

通过多来源的网络研究发现三个趋同趋势：

- **AI 基础设施/编排** 是增长最快的软件类别（AI 编排市场 2026 年估值约 135 亿美元，CAGR 22%+）
- **空间计算**（Vision Pro、WebXR）正在成熟，但缺乏杀手级企业应用
- 每个现有的 AI 工作流工具（LangSmith、n8n、Flowise、CrewAI）都是**扁平的 2D 仪表板**

### 概念：Nexus Spatial

一个空间计算中的 AI Agent 指挥中心 —— 一个 VisionOS + WebXR 应用，为编排、监控和与 AI agents 交互提供沉浸式 3D 指挥中心。用户可以将 agent 管道可视化为 3D 节点图，在空间面板中监控实时输出，在 3D 空间中用拖放构建工作流，并在共享空间环境中协作。

### 为什么这个 Agency 独具优势

该 agency 拥有深厚的空间计算专业知识（XR 开发者、VisionOS 工程师、Metal 专家、界面架构师），以及完整的工程、设计、营销和运营栈 —— 这对于一个既需要空间计算精通又需要企业软件严谨性的产品来说，是罕见的组合。

### 来源

- [Profitable SaaS Ideas 2026 (273K+ Reviews)](https://bigideasdb.com/profitable-saas-micro-saas-ideas-2026)
- [2026 SaaS and AI Revolution: 20 Top Trends](https://fungies.io/the-2026-saas-and-ai-revolution-20-top-trends/)
- [Top 21 Underserved Markets 2026](https://mktclarity.com/blogs/news/list-underserved-niches)
- [Fastest Growing Products 2026 - G2](https://www.g2.com/best-software-companies/fastest-growing)
- [PwC 2026 AI Business Predictions](https://www.pwc.com/us/en/tech-effect/ai-analytics/ai-predictions.html)

---

## 2. 市场验证

**Agent：** Product Trend Researcher

### 结论：有条件推进 —— 2D 优先，空间其次

### 市场规模

| 细分市场 | 2026 年价值 | 增长率 |
|---------|-----------|--------|
| AI 编排工具 | 135 亿美元 | 22.3% CAGR |
| 自主 AI Agents | 85 亿美元 | 45.8% CAGR，至 2030 年达 503 亿美元 |
| 扩展现实 (XR) | 106.4 亿美元 | 40.95% CAGR |
| 空间计算（广义） | 1700-2200 亿美元 | 因定义而异 |

### 竞争格局

**AI Agent 编排（均为 2D）：**

| 工具 | 优势 | UX 差距 |
|------|----------|--------|
| LangChain/LangSmith | 图形化编排，39 美元/用户/月 | 扁平仪表板；复杂图形在规模化时难以阅读 |
| CrewAI | 10 万+ 开发者，快速执行 | CLI 优先，最小可视化工具 |
| Microsoft Agent Framework | 企业集成 | 嵌入 Azure 门户，无独立 UI |
| n8n | 可视化工作流构建器，20-50 美元/月 | 2D 画布难以处理 agent 关系 |
| Flowise | 拖放 AI 流程 | 仅限线性流程，无多 agent 监控 |

**"Mission Control" 产品（新兴，均为 2D）：**
- cmd-deck：AI 编码 agents 的看板
- Supervity Agent Command Center：企业可观测性
- OpenClaw Command Center：Agent 集群管理
- Mission Control AI：合成工作者管理
- Mission Control HQ：小队式协调

**差距：** 产品要么是空间导向但非 AI 专注，要么是 AI 专注但扁平 2D。没有产品位于交叉点。

### Vision Pro 现实检查

- 已安装基数：全球约 100 万台（销量较发布时下降 95%）
- Apple 已将重心转向轻量级 AR 眼镜
- 仅存在约 3,000 个 VisionOS 专属应用
- **含义：** 不要以 VisionOS 为先导。以 Web 为先导，添加 WebXR，最后才是原生 VisionOS。

### WebXR 作为分发突破口

- Safari 在 2025 年末采纳了 WebXR Device API
- 2026 年 WebXR 采用率增长 40%
- WebGPU 在浏览器中提供接近原生的渲染
- Android XR 支持 WebXR 和 OpenXR 标准

### 目标用户画像和定价

| 层级 | 价格 | 目标用户 |
|------|-------|--------|
| Explorer | 免费 | 开发者、独立构建者（3 个 agents，WebXR 查看器） |
| Pro | 99 美元/用户/月 | 小型团队（25 个 agents，协作功能） |
| Team | 249 美元/用户/月 | 中型市场 AI 团队（无限 agents，分析） |
| Enterprise | 定制（2K-10K 美元/月） | 大型企业（SSO、RBAC、本地部署、SLA） |

### 建议的分阶段策略

1. **第 1-6 个月：** 构建具有 Three.js 2.5D 能力的优质 2D Web 仪表板。目标：50 个付费团队，6 万美元 MRR。
2. **第 6-12 个月：** 添加可选的 WebXR 空间模式（基于浏览器）。目标：200 个团队，30 万美元 MRR。
3. **第 12-18 个月：** 仅在空间需求得到验证时开发原生 VisionOS 应用。目标：500 个团队，100 万美元+ MRR。

### 关键风险

| 风险 | 严重程度 |
|------|----------|
| Vision Pro 已安装基数极小 | 高 |
| "空间解决方案寻找问题" —— 3D 实际上比 2D 好 10 倍吗？ | 高 |
| "mission control" 定位拥挤（已有 5+ 产品） | 中等 |
| 企业空间计算采用仍处于早期阶段 | 中等 |
| 跨 AI 框架的集成复杂性 | 中等 |

### 来源

- [MarketsandMarkets - AI Orchestration Market](https://www.marketsandmarkets.com/Market-Reports/ai-orchestration-market-148121911.html)
- [Deloitte - AI Agent Orchestration Predictions 2026](https://www.deloitte.com/us/en/insights/industry/technology/technology-media-and-telecom-predictions/2026/ai-agent-orchestration.html)
- [Mordor Intelligence - Extended Reality Market](https://www.mordorintelligence.com/industry-reports/extended-reality-xr-market)
- [Fintool - Vision Pro Production Halted](https://fintool.com/news/apple-vision-pro-production-halt)
- [MadXR - WebXR Browser-Based Experiences 2026](https://www.madxr.io/webxr-browser-immersive-experiences-2026.html)

---

## 3. 技术架构

**Agent：** Backend Architect

### 系统概述

一个 8 服务架构，具有清晰的职责边界，设计用于水平扩展和提供商无关的 AI 集成。

```
+------------------------------------------------------------------+
|                     CLIENT TIER                                   |
|  VisionOS Native (Swift/RealityKit)  |  WebXR (React Three Fiber) |
+------------------------------------------------------------------+
                              |
+-----------------------------v------------------------------------+
|                      API GATEWAY (Kong / AWS API GW)              |
|  Rate limiting | JWT validation | WebSocket upgrade | TLS        |
+------------------------------------------------------------------+
                              |
+------------------------------------------------------------------+
|                      SERVICE TIER                                 |
|  Auth | Workspace | Workflow | Orchestration (Rust) |             |
|  Collaboration (Yjs CRDT) | Streaming (WS) | Plugin | Billing    |
+------------------------------------------------------------------+
                              |
+------------------------------------------------------------------+
|                      DATA TIER                                    |
|  PostgreSQL 16 | Redis 7 Cluster | S3 | ClickHouse | NATS        |
+------------------------------------------------------------------+
                              |
+------------------------------------------------------------------+
|                    AI PROVIDER TIER                                |
|  OpenAI | Anthropic | Google | Local Models | Custom Plugins      |
+------------------------------------------------------------------+
```

### 技术栈

| 组件 | 技术 | 理由 |
|-----------|------------|-----------|
| 编排引擎 | **Rust** | 亚毫秒调度、零 GC 停顿、agent 沙箱的内存安全 |
| API 服务 | TypeScript / NestJS | CRUD 密集型服务的开发效率 |
| VisionOS 客户端 | Swift 6, SwiftUI, RealityKit | 一流的空间计算与 Liquid Glass |
| WebXR 客户端 | TypeScript, React Three Fiber | 生产级 WebXR 与 React 组件模型 |
| 消息代理 | NATS JetStream | 轻量级、精确一次交付、比 Kafka 简单 |
| 协作 | Yjs (CRDT) + WebRTC | 无冲突的并发 3D 图形编辑 |
| 主数据库 | PostgreSQL 16 | JSONB 用于灵活配置、行级安全用于租户隔离 |

### 核心数据模型

14 张表覆盖：
- **身份与访问：** users, workspaces, team_memberships, api_keys
- **工作流：** workflows, workflow_versions, nodes, edges
- **执行：** executions, execution_steps, step_output_chunks
- **协作：** collaboration_sessions, session_participants
- **凭证：** provider_credentials（AES-256-GCM 加密）
- **计费：** subscriptions, usage_records
- **审计：** audit_log（仅追加）

### 节点类型注册表

```
Built-in Node Types:
  ai_agent          -- Calls an AI provider with a prompt
  prompt_template   -- Renders a template with variables
  conditional       -- Routes based on expression
  transform         -- Sandboxed code snippet (JS/Python)
  input / output    -- Workflow entry/exit points
  human_review      -- Pauses for human approval
  loop              -- Repeats subgraph
  parallel_split    -- Fans out to branches
  parallel_join     -- Waits for branches
  webhook_trigger   -- External HTTP trigger
  delay             -- Timed pause
```

### WebSocket 频道

通过 WSS 进行实时流式传输，具有：
- 每频道序号用于排序
- 间隙检测与重放请求
- 当落后超过 1000 个事件时的快照恢复
- 针对低功耗设备的客户端节流

### 安全架构

| 层级 | 机制 |
|-------|-----------|
| 用户认证 | OAuth 2.0（GitHub、Google、Apple）+ 邮箱/密码 + 可选 TOTP MFA |
| API 密钥 | SHA-256 哈希、作用域限定、可选过期时间 |
| 服务间通信 | 通过服务网格的 mTLS |
| WebSocket 认证 | 30 秒过期的一次性票据 |
| 凭证存储 | 信封加密（AES-256-GCM + AWS KMS） |
| 代码沙箱 | gVisor/Firecracker 微虚拟机（无网络、256MB RAM、30 秒 CPU） |
| 租户隔离 | PostgreSQL 行级安全 + S3 IAM 策略 + NATS 主题范围限定 |

### 扩展目标

| 指标 | 第 1 年 | 第 2 年 |
|--------|--------|--------|
| 并发 agent 执行数 | 5,000 | 50,000 |
| WebSocket 连接数 | 10,000 | 100,000 |
| P95 API 延迟 | < 150ms | < 100ms |
| P95 WS 事件延迟 | < 80ms | < 50ms |

### MVP 阶段

1. **第 1-6 周：** 2D Web 编辑器、顺序执行、OpenAI + Anthropic 适配器
2. **第 7-12 周：** WebXR 3D 模式、并行执行、手势追踪、RBAC
3. **第 13-20 周：** 多用户协作、VisionOS 原生、计费
4. **第 21-30 周：** 企业 SSO、插件 SDK、SOC 2、规模加固

---

## 4. 品牌策略

**Agent：** Brand Guardian

### 定位

**品类创造优于品类竞争。** Nexus Spatial 定义了一个新品类 —— **Spatial AI Operations (SpatialAIOps)** —— 而不是在拥挤的 AI 可观测性仪表板空间中争夺位置。

**定位陈述：** 对于管理复杂 AI agent 工作流的技术团队，Nexus Spatial 是提供 agent 编排空间感知的沉浸式 3D 指挥中心，与扁平的 2D 仪表板不同，因为空间计算将监控从阅读仪表板转变为身临其境地感知你的基础设施。

### 名称验证

"Nexus Spatial" **已验证为强有力的名称：**
- "Nexus" 与 NEXUS 编排框架相连（Network of EXperts, Unified in Strategy）
- "Nexus" 本身意为"中央连接点" —— 非常适合指挥中心
- "Spatial" 是 Apple 和行业已标准化的行业标准描述符
- 语音平衡：三个音节，然后两个音节
- **需要行动：** 在尼斯分类第 9、42 和 38 类进行商标清算

### 品牌个性：指挥官

| 特质 | 表达方式 | 避免 |
|-------|------------|------|
| **权威** | 清晰、直接、技术精确 | 炒作、最高级、模糊的未来主义 |
| **沉稳** | 简洁的设计、适度的节奏、留白 | 为了紧迫而紧迫、混乱 |
| **先锋** | 安静的自豪、对新范式的不张扬引用 | "革命性"、"改变游戏规则" |
| **精准** | 确切的规格、真实的指标、诚实的要求 | 模糊的声明、营销术语 |
| **亲和** | 自然的交互语言、空间隐喻 | 居高临下、设门槛 |

### 标语（排名）

1. **"Agent 时代的任务控制中心"** —— 推荐首选
2. "在空间中查看你的 Agents"
3. "在三维中编排"
4. "AI 运维变得空间化"
5. "指挥中心。在空间中重新构想。"
6. "你的仪表板缺失的维度"
7. "AI Agents 值得比平面屏幕更多"

### 色彩系统

| 颜色 | Hex | 用途 |
|-------|-----|-------|
| Deep Space Indigo | `#1B1F3B` | 基础深色画布、背景 |
| Nexus Blue | `#4A7BF7` | 签名品牌色、主要操作 |
| Signal Cyan | `#00D4FF` | 空间高亮、数据连接 |
| Command Green | `#00E676` | 健康系统、成功 |
| Alert Amber | `#FFB300` | 警告、需要关注 |
| Critical Red | `#FF3D71` | 错误、失败 |

使用比例：Deep Space Indigo 60%、Nexus Blue 25%、Signal Cyan 10%、语义色 5%。

### 字体排印

- **主要：** Inter（UI、正文、标签）
- **等宽：** JetBrains Mono（代码、日志、agent 输出）
- **展示：** Space Grotesk（仅营销标题）

### Logo 概念

三个探索方向：

1. **Spatial Nexus Mark** —— 会聚线条在发光的中心节点交汇，带有微妙的透视深度
2. **Dimensional Window** —— 风格化视口，透视线创造看向 3D 空间的效果
3. **Orbital Array** —— 围绕中心点的轨道环，暗示协调中的 agents 在运动

### 品牌价值观

- **空间真实性** —— 系统状态的诚实呈现，无装饰性平滑
- **运维严肃性** —— 为生产而建，而非演示
- **维度包容性** —— WebXR 确保空间价值对每个人都可访问
- **复杂中的从容** —— 系统越复杂，界面越平静

### 设计令牌

```css
:root {
  --nxs-deep-space:       #1B1F3B;
  --nxs-blue:             #4A7BF7;
  --nxs-cyan:             #00D4FF;
  --nxs-green:            #00E676;
  --nxs-amber:            #FFB300;
  --nxs-red:              #FF3D71;
  --nxs-void:             #0A0E1A;
  --nxs-slate-900:        #141829;
  --nxs-slate-700:        #2A2F45;
  --nxs-slate-500:        #4A5068;
  --nxs-slate-300:        #8B92A8;
  --nxs-slate-100:        #C8CCE0;
  --nxs-cloud:            #E8EBF5;
  --nxs-white:            #F8F9FC;
  --nxs-font-primary:     'Inter', sans-serif;
  --nxs-font-mono:        'JetBrains Mono', monospace;
  --nxs-font-display:     'Space Grotesk', sans-serif;
}
```

---

## 5. Go-to-Market 与增长

**Agent：** Growth Hacker

### 北极星指标

**每周活跃管道 (WAP)** —— 过去 7 天内至少有一次空间交互的唯一 agent 管道。既捕获创建又捕获参与，与价值相关，且不可被操控。

### 定价

| 层级 | 年付 | 月付 | 目标 |
|------|--------|---------|------|
| Explorer | 免费 | 免费 | 3 个管道、WebXR 预览、社区 |
| Pro | 29 美元/用户/月 | 39 美元/用户/月 | 无限管道、VisionOS、30 天历史 |
| Team | 59 美元/用户/月 | 79 美元/用户/月 | 协作、RBAC、SSO、90 天历史 |
| Enterprise | 定制（约 150 美元+） | 定制 | 专属基础设施、SLA、本地部署选项 |

策略：14 天反向试用（先 Pro 功能，然后降级到免费）。目标 5-8% 免费转付费转化率。

### 三阶段 GTM

**第 1 阶段：创始人主导销售（第 1-3 个月）**
- 目标：使用 LangChain/CrewAI 并拥有 Vision Pro 的初创公司个人 AI 工程师
- 策略：私信 200 位高知名度 AI 工程师、每周公开构建帖子、30 秒演示片段
- 渠道：X/Twitter、LinkedIn、AI 专注的 Discord 服务器、Reddit

**第 2 阶段：开发者社区（第 4-6 个月）**
- Product Hunt 发布（定在此阶段，非第 1 阶段）
- Hacker News Show HN、Dev.to 文章、会议演讲
- 与热门 AI 框架的集成公告

**第 3 阶段：企业（第 7-12 个月）**
- Apple 企业推荐渠道、LinkedIn ABM 活动
- 企业案例研究、分析师简报（Gartner、Forrester）
- 首位企业 AE 招聘、SOC 2 合规

### 增长飞轮

1. **"惊叹因素"演示飞轮** —— 空间演示天生具有可分享性。一键"分享空间预览"生成 WebXR 链接或视频。目标 K = 0.3-0.5。
2. **模板市场** —— 高级用户发布管道模板，通过搜索发现，驱动新注册。
3. **协作席位扩展** —— 一位工程师采用，分享给队友，团队扩展到付费计划（Slack/Figma 策略）。
4. **集成驱动发现** —— 在 LangChain、n8n、OpenAI/Anthropic 合作伙伴目录中列出。

### 开源策略

**开源 (Apache 2.0)：**
- `nexus-spatial-sdk` —— TypeScript/Python SDK，用于连接 agent 框架
- `nexus-webxr-components` —— React Three Fiber 组件库，用于 3D 管道
- `nexus-agent-schemas` —— 标准化 schema，用于在 3D 中表示 agent 管道

**保持专有：** VisionOS 原生应用、协作引擎、企业功能、托管基础设施。

### 收入目标

| 指标 | 第 6 个月 | 第 12 个月 |
|--------|---------|----------|
| MRR | 8K-15K 美元 | 50K-80K 美元 |
| 免费账户 | 5,000 | 15,000 |
| 付费席位 | 300 | 1,200 |
| Discord 成员 | 2,000 | 5,000 |
| GitHub Stars (SDK) | 500 | 2,000 |

### 首个 5 万美元预算

| 类别 | 金额 | % |
|----------|--------|---|
| 内容制作 | 12,000 美元 | 24% |
| 开发者关系 | 10,000 美元 | 20% |
| 付费获客测试 | 8,000 美元 | 16% |
| 社区与工具 | 5,000 美元 | 10% |
| Product Hunt 与发布 | 3,000 美元 | 6% |
| 开源维护 | 3,000 美元 | 6% |
| PR 与外联 | 4,000 美元 | 8% |
| 合作伙伴 | 2,000 美元 | 4% |
| 储备金 | 3,000 美元 | 6% |

### 关键合作伙伴

- **第 1 层（关键）：** Anthropic、OpenAI —— 一流 API 集成、合作伙伴计划列表
- **第 2 层（采用）：** LangChain、CrewAI、n8n —— 框架集成、社区交叉传播
- **第 3 层（平台）：** Apple —— Vision Pro 开发者套件、App Store 推荐、WWDC
- **第 4 层（生态）：** GitHub、Hugging Face、Docker —— 开发者平台集成

### 来源

- [AI Orchestration Market Size - MarketsandMarkets](https://www.marketsandmarkets.com/Market-Reports/ai-orchestration-market-148121911.html)
- [Spatial Computing Market - Precedence Research](https://www.precedenceresearch.com/spatial-computing-market)
- [How to Price AI Products - Aakash Gupta](https://www.news.aakashg.com/p/how-to-price-ai-products)
- [Product Hunt Launch Guide 2026](https://calmops.com/indie-hackers/product-hunt-launch-guide/)

---

## 6. 客户支持蓝图

**Agent：** Support Responder

### 支持层级结构

| 属性 | Explorer (免费) | Builder (Pro) | Command (企业) |
|-----------|-----------------|---------------|---------------------|
| 首次响应 SLA | 尽力而为（48 小时） | 4 小时（工作时间） | 30 分钟（P1）、2 小时（P2） |
| 解决 SLA | 5 个工作日 | 24 小时（P1/P2）、72 小时（P3） | 4 小时（P1）、12 小时（P2） |
| 渠道 | 社区、知识库、AI 助手 | + 实时聊天、邮件、视频（2 次/月） | + 专属 Slack、指定 CSE、24/7 |
| 范围 | 一般问题、文档 | 技术故障排除、集成 | 全面集成、定制设计、合规 |

### 优先级定义

- **P1 紧急：** 编排宕机、数据丢失风险、安全漏洞
- **P2 高：** 主要功能降级、存在变通方案
- **P3 中：** 非阻塞问题、小故障
- **P4 低：** 功能请求、外观问题

### Nexus Guide：AI 驱动的产品内支持

突出的设计决策：支持 agent 作为可见节点存在于**用户的空间工作区内**。它完全了解用户的布局、活跃 agents 和最近的错误。

**能力：**
- 关于功能的自然语言问答
- 实时 agent 诊断（"Agent X 为什么慢？"）
- 配置建议（"你的拓扑结构作为网状会性能更好"）
- 引导式空间故障排除演练
- 工单创建并自动附加上下文

**自愈：**

| 场景 | 检测 | 自动解决 |
|----------|-----------|-----------------|
| Agent 无限循环 | CPU/token 飙升 | 使用最后良好配置终止并重启 |
| 渲染帧率下降 | FPS 低于阈值 | 降低视觉保真度、建议关闭面板 |
| 凭证过期 | API 401 响应 | 提示重新认证、优雅暂停 agents |
| 通信超时 | 延迟飙升 | 通过备用路径重新路由消息 |

### 引导流程

基于用户画像的自适应引导：

| AI 经验 | 空间经验 | 路径 |
|---------------|-------------------|------|
| 低 | 低 | 完整引导导览（20 分钟） |
| 高 | 低 | 空间聚焦（12 分钟） |
| 低 | 高 | Agent 聚焦（12 分钟） |
| 高 | 高 | 快速设置（5 分钟） |

关键第一步：在任何产品交互前进行 60 秒空间校准（手势追踪、凝视、舒适度检查）。

**激活里程碑**（用户"完成引导"的标准）：
- 创建至少一个自定义 agent
- 在拓扑中连接两个或更多 agents
- 锚定至少一个监控仪表板
- 返回进行第三次会话

### 团队建设

| 阶段 | ��数 | 角色 |
|-------|-----------|------|
| 第 0-6 个月 | 4 | CX 负责人、2 名支持工程师、技术文档工程师 |
| 第 6-12 个月 | 8 | + 2 名支持工程师、CSE、社区经理、运维分析师 |
| 第 12-24 个月 | 16 | + 4 名工程师（24/7）、空间专家、集成专家、知识库管理员、工程经理 |

### 社区：Discord 优先

```
NEXUS SPATIAL DISCORD
  INFORMATION: #announcements, #changelog, #status
  SUPPORT: #help-getting-started, #help-agents, #help-spatial
  DISCUSSION: #general, #show-your-workspace, #feature-requests
  PLATFORMS: #visionos, #webxr, #api-and-sdk
  EVENTS: office-hours (weekly voice), community-demos (monthly)
  PRO MEMBERS: #pro-lounge, #beta-testing
  ENTERPRISE: per-customer private channels
```

**冠军计划（"Nexus Navigators"）：** 5-10 位初始高级用户，获得 Navigator 徽章、与产品团队的直接 Slack、免费 Pro 层级、早期功能访问权限、年度峰会。

---

## 7. UX 研究与设计方向

**Agent：** UX Researcher

### 用户画像

**Maya Chen —— AI 平台工程师（32 岁，旧金山）**
- 管理 15-30 个活跃 agent 工作流，使用 n8n + LangSmith
- 40% 的时间用于通过日志检查调试 agent 故障
- 对空间计算持怀疑态度："这真的更快，还是只是更酷？"
- 主要需求：将平均诊断时间从 45 分钟减少到 10 分钟以内

**David Okoro —— 技术产品经理（38 岁，伦敦）**
- 审查和批准 agent 工作流设计，向 C 级高管汇报
- 无法有意义地参与工作流评审，因为工具需要代码级理解
- 主要需求：在不需要阅读代码的情况下理解和传达 agent 架构

**Dr. Amara Osei —— 研究科学家（45 岁，苏黎世）**
- 设计带 A/B 对比的多 agent 研究工作流
- 同一管道有 12 个变体，没有好的比较方式
- 主要需求：在 3D 空间中并排比较变体管道

**Jordan Rivera —— 创意技术专家（27 岁，奥斯汀）**
- 日常 Vision Pro 用户，构建 AI 驱动的艺术装置
- 希望工具感觉像乐器，而不是仪表板
- 主要需求：快速构建 agent 工作流并获得即时空间反馈

### 关键发现：调试是杀手级用例

在图形结构上进行运行时追踪的空间叠加解决了一个真正的、量化的痛点，这是任何 2D 工具都无法很好处理的。这个工作流应该获得最多的设计和工程投入。

### 关键设计洞察

空间为**结构化**任务（放置、连接、重排节点）增加价值，但为**参数化**任务（文本输入、配置）制造摩擦。界面必须无缝融合空间和 2D 模式 —— 锚定到空间位置的 2D 面板。

### 7 条设计原则

1. **空间必须证明其价值** —— 如果 2D 更清晰，就用 2D。每次评审都应问："扁平会不会更好？"
2. **先可扫视，再可检查** —— 关键信息通过颜色、大小、运动、位置在 2 秒内可感知
3. **免手是基准** —— 凝视 + 语音覆盖所有阅读/导航操作；手增加精度但不��必需的
4. **尊重认知引力** —— 扩展 2D 心智模型（从左到右流程），不要替换它们；Z 轴增加层次
5. **渐进式空间复杂度** —— 新用户从近乎 2D 开始；空间能力随信心增长而展现
6. **物理隐喻，数字能力** —— 节点被"拾起"（物理）但也可以复制和版本化（数字）
7. **静默是功能** —— 健康系统感觉平静；颜色和运动信号偏离正常状态

### 导航范式：4 级语义缩放

| 级别 | 看到的内容 |
|-------|-------------|
| Fleet View | 所有工作流作为抽象形状，按状态颜色编码 |
| Workflow View | 带标签和连接的节点图 |
| Node View | 展开的配置、最近的 I/O、状态指标 |
| Trace View | 完整执行追踪与数据检查 |

### 竞品 UX 概览

| 能力 | n8n | Flowise | LangSmith | Langflow | Nexus Spatial 目标 |
|-----------|-----|---------|-----------|----------|---------------------|
| 可视化工作流构建 | A | B+ | N/A | A | A+（空间） |
| 调试/追踪 | C+ | C | A | B | A+（空间叠加） |
| 监控 | B | C | A | B | A（空间集群） |
| 协作 | D | D | C | D | A（空间共存） |
| 大型工作流可扩展性 | C | C | B | C | A（3D 空间） |

### 无障碍要求

- 每个交互至少可通过两种模态实现
- 不单独通过颜色传达信息
- 高对比度模式、减少运动模式、深度扁平化模式
- 屏幕阅读器兼容性与空间元素描述
- 每 20-30 分钟的会话时长警告
- 所有关键任务可坐着、单手、在 30 度运动锥内完成

### 研究计划（16 周）

| 阶段 | 周数 | 研究 |
|-------|-------|------|
| 基础 | 1-4 | 心智模型访谈（15-20 名参与者）、竞品任务分析 |
| 概念验证 | 5-8 | Wizard-of-Oz 空间原型测试、信息架构的 3D 卡片分类 |
| 可用性测试 | 9-14 | 首次使用体验（20 名用户）、4 周纵向日记研究、配对协作测试 |
| 无障碍审计 | 12-16 | 专家启发式评估、残障用户测试 |

---

## 8. 项目执行计划

**Agent：** Project Shepherd

### 时间线：35 周（2026 年 3 月 9 日 — 11 月 6 日）

| 阶段 | 周数 | 持续时间 | 目标 |
|-------|-------|----------|------|
| 发现与研究 | W1-3 | 3 周 | 验证可行性、定义范围 |
| 基础 | W4-9 | 6 周 | 核心基础设施、两个平台外壳、设计系统 |
| MVP 构建 | W10-19 | 10 周 | 单用户 agent 指挥中心与编排 |
| Beta | W20-27 | 8 周 | 协作、打磨、加固、50-100 名 beta 用户 |
| 发布 | W28-31 | 4 周 | App Store + Web 发布、营销推动 |
| 规模化 | W32-35+ | 持续 | 插件市场、高级功能、增长 |

### 关键里程碑：第 12 周（5 月 29 日）

**首次端到端工作流执行。** 用户在 3D 中创建并运行 3 节点 agent 工作流。这是产品证明其核心价值主张的时刻。如果这个延迟，所有下游都会推迟。

### 前 6 个冲刺（65 个任务）

**冲刺 1（3 月 9-20 日）：** VisionOS SDK 审计、WebXR 兼容性矩阵、编排引擎可行性、利益相关者访谈、两个平台的临时原型。

**冲刺 2（3 月 23 日 - 4 月 3 日）：** 架构决策记录、MoSCoW 确定 MVP 范围、PRD v1.0、空间 UI 模式研究、交互模型定义、设计系统启动。

**冲刺 3（4 月 6-17 日）：** Monorepo 设置、认证服务（OAuth2）、数据库 schema、API 网关、VisionOS Xcode 项目初始化、WebXR 项目初始化、CI/CD 流水线。

**冲刺 4（4 月 20 日 - 5 月 1 日）：** WebSocket 服务器 + 客户端 SDK、空间窗口管理、3D 组件库、手势追踪输入层、团队 CRUD、集成测试。

**冲刺 5（5 月 4-15 日）：** 编排引擎核心（Rust）、agent 状态机、节点图渲染器（两个平台）、插件接口 v0、OpenAI 提供商插件。

**冲刺 6（5 月 18-29 日）：** 工作流持久化 + 版本控制、DAG 执行、实时执行��视化、Anthropic 提供商插件、眼动追踪集成、空间音频。

### 团队分配

跨阶段运作的 5 个小组：

| 小组 | 核心成员 | 活跃阶段 |
|-------|-------------|---------------|
| Core Architecture | Backend Architect, XR Interface Architect, Senior Dev, VisionOS Engineer | 发现到 MVP |
| Spatial Experience | XR Immersive Dev, XR Cockpit Specialist, Metal Engineer, UX Architect, UI Designer | 基础到 Beta |
| Orchestration | AI Engineer, Backend Architect, Senior Dev, API Tester | MVP 到 Beta |
| Platform Delivery | Frontend Dev, Mobile App Builder, VisionOS Engineer, DevOps | MVP 到发布 |
| Launch | Growth Hacker, Content Creator, App Store Optimizer, Visual Storyteller, Brand Guardian | Beta 到规模化 |

### 前 5 大风险

| 风险 | 概率 | 影响 | 缓解措施 |
|------|------------|--------|------------|
| Apple 拒绝 VisionOS 应用 | 中 | 关键 | 第 4 周接触 Apple 开发者关系，第 20 周前预审 |
| WebXR 浏览器碎片化 | 高 | 高 | 第 1 周浏览器支持矩阵，自动化跨浏览器测试 |
| 多用户同步冲突 | 中 | 高 | 从一开始使用基于 CRDT 的同步（Yjs），在基础阶段原型验证 |
| 编排无法扩展 | 中 | 关键 | 第一天就水平扩展，第 22 周负载测试达 10 倍 |
| RealityKit 100+ 节点性能 | 中 | 高 | 早期性能分析、实现 LOD 剔除、实例化渲染 |

### 预算：121,500 美元 — 155,500 美元（非人员）

| 类别 | 估算成本 |
|----------|---------------|
| 云基础设施（35 周） | 35,000 - 45,000 美元 |
| 硬件（3 台 Vision Pro、2 台 Quest 3、Mac Studio） | 17,500 美元 |
| 许可证和服务 | 15,000 - 20,000 美元 |
| 外部服务（法律、安全、PR） | 30,000 - 45,000 美元 |
| AI API 成本（开发/测试） | 8,000 美元 |
| 应急储备（15%） | 16,000 - 20,000 美元 |

---

## 9. 空间界面架构

**Agent：** XR Interface Architect

### 指挥剧场

工作区组织为围绕用户的曲线剧场：

```
                        OVERVIEW CANOPY
                     (pipeline topology)
                    ~~~~~~~~~~~~~~~~~~~~~~~~
                   /                        \
                  /     FOCUS ARC (120 deg)   \
                 /    primary node graph work   \
                /________________________________\
               |                                  |
    LEFT       |        USER POSITION             |       RIGHT
    UTILITY    |        (origin 0,0,0)            |       UTILITY
    RAIL       |                                  |       RAIL
               |__________________________________|
                \                                /
                 \      SHELF (below sightline) /
                  \   agent status, quick tools/
                   \_________________________ /
```

- **Focus Arc**（120 度，1.2-2.0m）：主要节点图工作区
- **Overview Canopy**（上方，2.5-4.0m）：缩略管道拓扑 + 健康热力图
- **Utility Rails**（左/右两侧）：Agent 库、监控、日志
- **Shelf**（视线以下，0.8-1.0m）：运行/停止、撤销/重做、快捷工具

### 三层深度系统

| 层级 | 深度 | 内容 | 不透明度 |
|-------|-------|---------|---------|
| 前景 | 0.8 - 1.2m | 活动面板、检查器、模态框 | 100% |
| 中景 | 1.2 - 2.5m | 节点图、连接、工作区 | 100% |
| 背景 | 2.5 - 5.0m | 概览地图、环境状态 | 40-70% |

### 3D 节点图

**数据流向用户流动。** 节点按执行顺序沿 Z 轴排列：

```
USER (here)
  z=0.0m   [Output Nodes]     -- 结果
  z=0.3m   [Transform Nodes]  -- 处理器
  z=0.6m   [Agent Nodes]      -- LLM 调用
  z=0.9m   [Retrieval Nodes]  -- RAG、API
  z=1.2m   [Input Nodes]      -- 触发器
```

并行分支水平展开（X 轴）。条件分支垂直展开（Y 轴）。

**节点表示（3 个 LOD）��**
- **LOD-0**（静止，>1.5m）：12x8cm 毛玻璃矩形，带类型图标、名称、状态发光
- **LOD-1**（悬停，400ms 凝视）：展开至 14x10cm，显示端口、上次运行信息
- **LOD-2**（选中）：滑至前景，展开为 30x40cm 详情面板，支持实时配置编辑

**连接作为发光管道：**
- 静止时直径 4mm，传输数据时 8mm
- 按数据类型颜色编码（白色=文本、青色=结构化、品红=图像、琥珀色=音频、绿色=工具调用）
- 动画粒子显示流向和速度
- 同层之间超过 3 条并行时自动捆绑

### 7 种 Agent 状态

| 状态 | 边缘发光 | 内部 | 声音 | 粒子 |
|-------|-----------|----------|-------|-----------|
| Idle | 稳定绿色，低亮度 | 静态毛玻璃 | 无 | 无 |
| Queued | 脉冲琥珀色，1Hz | 微弱旋转 | 无 | 输入端缓慢漂移 |
| Running | 稳定蓝色，中等亮度 | 动画微光 | 柔和空间嗡鸣 | 连接上快速流动 |
| Streaming | 蓝色 + 输出流 | 微光 + 文本片段 | 嗡鸣 | 文本片段向前流动 |
| Completed | 白色闪烁，然后绿色 | 静态 | 完成提示音 | 无 |
| Error | 脉冲红色，2Hz | 红色色调 | 警报音（一次） | 无 |
| Paused | 稳定琥珀色 | 冻结帧 + 暂停图标 | 无 | 冻结在原地 |

### 交互模型

| 动作 | VisionOS | WebXR 控制器 | 语音 |
|--------|----------|-------------------|-------|
| 选择节点 | 凝视 + 捏合 | 指向射线 + 触发器 | "选择 [名称]" |
| 移动节点 | 捏合 + 拖动 | 握持 + 移动 | -- |
| 连接端口 | 捏合端口 + 拖动 | 触发端口 + 拖动 | "连接 [A] 到 [B]" |
| 平移工作区 | 双手拖动 | 摇杆 | "向左/右平移" |
| 缩放 | 双手展开/捏合 | 摇杆推/拉 | "放大/缩小" |
| 检查节点 | 捏合 + 拉向自己 | 双击触发器 | "检查 [名称]" |
| 运行管道 | 点击 Shelf 按钮 | 触发按钮 | "运行管道" |
| 撤销 | 双指双击 | B 按钮 | "撤销" |

### 协作存在感

每个协作者表示为：
- **头部代理：** 带头像的半透明球体，随头部方向旋转
- **手部代理：** 显示捏合/抓取状态的幽灵手模型
- **凝视锥：** 微妙的 10 度锥体显示他们正在看哪里
- **名称标签：** Billboard 渲染，显示当前动作（"正在编辑节点 X"）

**冲突解决：** 首位编辑者获得写锁；第二位看到"已被 [名称] 锁定"，可选择请求访问或复制节点。

### 自适应布局

| 环境 | 节点比例 | 最大 LOD-2 节点数 | 图形 Z 展开 |
|-------------|-----------|-----------------|----------------|
| VisionOS Window | 4x3cm | 5 | 0.05m/层 |
| VisionOS Immersive | 12x8cm | 15 | 0.3m/层 |
| WebXR Desktop | 120x80px | 8（覆盖层） | 透视投影 |
| WebXR Immersive | 12x8cm | 12 | 0.3m/层 |

### 过渡编排

所有过渡都服务于寻路。主要过渡最多 600ms，次要 200ms，选择 0ms。

| 过渡 | 持续时间 | 关键运动 |
|-----------|----------|------------|
| 概览到聚焦 | 600ms | 相机漂移到目标，其他区域淡出至 30% |
| 聚焦到详情 | 500ms | 节点向前滑动、展开、连接高亮 |
| 详情到概览 | 600ms | 面板折叠、节点后退、完整拓扑可见 |
| 区域切换 | 500ms | 当前区域侧向滑出，新区域滑入 |
| 窗口到沉浸式 | 1000ms | 边界溶解、节点展开到完整空间位置 |

### 舒适措施

- 无用户操作时不发生相机移动
- 稳定地平线（水平面永不倾斜）
- 主要交互在 0.8-2.5m 内，眼线上下 +/-15 度
- 45 分钟后休息提示（环境光变化，非模态）
- 快速移动时的外围晕影
- 所有必要控件可在手臂自然下垂时访问（手腕/手指）

---

## 10. 跨 Agent 综合

### 所有 8 个 Agents 的共识点

1. **2D 优先，空间其次。** 每个 agent 都独立得出这个结论。先构建优秀的 Web 仪表板，然后逐步添加空间能力。

2. **调试是杀手级用例。** Product Researcher、UX Researcher 和 XR Interface Architect 都聚焦于此：在图形结构上进行运行时追踪的空间叠加是 3D 真正胜过 2D 的地方。

3. **WebXR 优于 VisionOS 用于初始覆盖。** Vision Pro 约 100 万的已安装基数无法支撑业务。浏览器中的 WebXR 是分发突破口。

4. **"作战室"协作场景。** 多个 agents 强调协作事件响应是最强的空间价值主张 —— 团队进入��享 3D 空间一起调试失败的管道。

5. **渐进式揭示至关重要。** UX Research、Spatial UI 和 Support 都强调空间复杂度必须逐步展现，绝不能倾倒给首次用户。

6. **语音作为高级用户加速器。** UX Researcher 和 XR Interface Architect 都识别出语音命令是"空间计算的命令行" —— 对无障碍和专家效率至关重要。

### 需要解决的关键张力

| 张力 | 观点 A | 观点 B | 需要解决 |
|---------|-----------|-----------|-------------------|
| **定价** | Growth Hacker：29-59 美元/用户/月 | Trend Researcher：99-249 美元/用户/月 | Beta 中 A/B 测试 |
| **VisionOS 优先级** | Architecture：第 3 阶段（第 13 周+） | Spatial UI：完整规范已就绪 | 先构建 WebXR，验证后再 VisionOS |
| **编排语言** | Architecture：Rust | Project Plan：未指定 | Rust 是性能关键 DAG 执行的正确选择 |
| **MVP 范围** | Architecture：第 1 阶段仅 2D | Brand：以空间为主导 | 2D 优先，但确保每个演示都有空间 |
| **社区平台** | Support：Discord 优先 | Marketing：Discord + 开源 | 两者兼顾 —— Discord 用于社区，GitHub 用于开发者参与 |

### 本实践展示了什么

这份发现文档由 8 个专业化 agents 并行产出，每个都为共同目标带来深厚的领域专业知识。Agents 独立得出一致的结论，同时揭示单一通才难以产生的领域特定洞察：

- **Product Trend Researcher** 发现了令人清醒的 Vision Pro 销售数据，重构了整个策略
- **Backend Architect** 设计了任何以营销为中心的团队都不会考虑的 Rust 编排引擎
- **Brand Guardian** 创造了一个新品类（"SpatialAIOps"）而非在现有品类中竞争
- **UX Researcher** 发现空间计算为参数化任务制造摩擦 —— 一个反直觉的发现
- **XR Interface Architect** 设计了"数据流向你流动"的拓扑，映射到自然空间认知
- **Project Shepherd** 识别了可能破坏整个时间线的三个关键瓶颈角色
- **Growth Hacker** 设计了特定于空间计算天生可分享性的病毒循环
- **Support Responder** 将产品自身的 AI 能力转化为支持差异化优势

结果是一份全面的、跨职能的产品计划，可以作为实际开发的基础 —— 由一组 AI agents 在单次会话中协同产出。