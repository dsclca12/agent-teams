# 示例

本目录包含示例输出，展示了如何协调 agency 的 agents 协同完成实际任务。

## 为什么需要这些示例

agency-agents 仓库定义了数十个专业化的 agents，涵盖工程、设计、营销、产品、支持、空间计算和项目管理等领域。但仅凭 agent 定义并不能展示当你**同时部署所有 agents** 执行单一任务时会发生什么。

这些示例回答了这个问题：*"当整个 agency 协作时，实际上是什么样的？"*

## 内容

### [nexus-spatial-discovery.md](./nexus-spatial-discovery.md)

**内容：** 一次完整的产品发现实践，8 个 agents 并行工作，评估软件机会并生成统一的计划。

**场景：** 网络研究在 AI agent 编排和空间计算的交汇处发现了一个机会。随后整个 agency 被同时部署以产出：

- 市场验证和竞争分析
- 技术架构（8 服务系统设计，完整的 SQL schema）
- 品牌策略和视觉识别
- Go-to-market 和增长计划
- 客户支持运营蓝图
- UX 研究计划（包含用户画像和用户旅程地图）
- 35 周项目执行计划（65 个冲刺任务）
- 空间界面架构规范

**使用的 Agents：**
| Agent | 角色 |
|-------|------|
| Product Trend Researcher | 市场验证、竞争格局 |
| Backend Architect | 系统架构、数据模型、API 设计 |
| Brand Guardian | 定位、视觉识别、命名 |
| Growth Hacker | GTM 策略、定价、发布计划 |
| Support Responder | 支持层级、引导、社区 |
| UX Researcher | 用户画像、用户旅程地图、设计原则 |
| Project Shepherd | 阶段计划、冲刺、风险登记 |
| XR Interface Architect | 空间 UI 规范 |

**核心收获：** 所有 8 个 agents 并行运行，产出了连贯、相互引用的计划，无需协调开销。输出展示了 agency 在单次会话中从"发现机会"到"提供完整蓝图"的能力。

## 添加新示例

如果你运行了一个有趣的多 agent 实践，考虑将其添加到这里。好的示例应该展示：

- 多个 agents 在共同目标上协作
- agency 能力的广度
- agent 定义的实际应用价值