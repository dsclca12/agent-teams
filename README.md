# 🎭 The Agency：随时准备改变您工作流程的 AI 专家团队

> **触手可及的完整 AI 代理机构** —— 从前端开发专家到 Reddit 社区运营高手，从趣味注入师到现实核查员。每个代理都是拥有独特个性、专业流程和成熟交付成果的领域专家。

[![GitHub stars](https://img.shields.io/github/stars/msitarzewski/agency-agents?style=social)](https://github.com/msitarzewski/agency-agents)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
[![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-pink?logo=github)](https://github.com/sponsors/msitarzewski)

---

## 🚀 这是什么？

源于一次 Reddit 帖子和数月的迭代打磨，**The Agency** 是一个不断增长的精心设计的 AI 代理人格集合。每个代理都：

- **🎯 高度专业化**：深入领域专业知识（而非通用提示模板）
- **🧠 个性驱动**：独特的声音、沟通风格和工作方式
- **📋 交付导向**：真实代码、流程和可衡量的成果
- **✅ 生产就绪**：经过实战检验的工作流程和成功指标

**把它想象成**：组建您的梦之队，只不过他们是永不休息、从不抱怨、始终交付的 AI 专家。

---

## ⚡ 快速开始

### 方式一：配合 Claude Code 使用（推荐）

```bash
# 复制代理到您的 Claude Code 目录
cp -r agency-agents/* ~/.claude/agents/

# 现在在您的 Claude Code 会话中激活任意代理：
# "Hey Claude, activate Frontend Developer mode and help me build a React component"
```

### 方式二：作为参考使用

每个代理文件包含：
- 身份与个性特征
- 核心使命与工作流程
- 带代码示例的技术交付成果
- 成功指标与沟通风格

浏览下方代理列表，复制/适配您需要的代理！

### 方式三：配合其他工具使用（Cursor、Aider、Windsurf、Gemini CLI、OpenCode）

```bash
# 步骤一 —— 为所有支持的工具生成集成文件
./scripts/convert.sh

# 步骤二 —— 交互式安装（自动检测已安装的工具）
./scripts/install.sh

# 或直接指定特定工具
./scripts/install.sh --tool cursor
./scripts/install.sh --tool aider
./scripts/install.sh --tool windsurf
```

详见下方的[多工具集成](#-多工具集成)章节。

---

## 🎨 代理团队名册

### 💻 工程部门

一次提交，构建未来。

| 代理 | 专业领域 | 适用场景 |
|-------|-----------|-------------|
| 🎨 [前端开发工程师](engineering/engineering-frontend-developer.md) | React/Vue/Angular、UI 实现、性能优化 | 现代网络应用、像素级完美的 UI、Core Web Vitals 优化 |
| 🏗️ [后端架构师](engineering/engineering-backend-architect.md) | API 设计、数据库架构、可扩展性 | 服务端系统、微服务、云基础设施 |
| 📱 [移动应用开发工程师](engineering/engineering-mobile-app-builder.md) | iOS/Android、React Native、Flutter | 原生和跨平台移动应用程序 |
| 🤖 [AI 工程师](engineering/engineering-ai-engineer.md) | 机器学习模型、部署、AI 集成 | 机器学习功能、数据管道、AI 驱动的应用 |
| 🚀 [DevOps 自动化工程师](engineering/engineering-devops-automator.md) | CI/CD、基础设施自动化、云运维 | 流水线开发、部署自动化、监控 |
| ⚡ [快速原型开发工程师](engineering/engineering-rapid-prototyper.md) | 快速 POC 开发、MVP | 快速概念��证、黑客马拉松项目、快速迭代 |
| 💎 [高级开发工程师](engineering/engineering-senior-developer.md) | Laravel/Livewire、高级设计模式 | 复杂实现、架构决策 |
| 🔒 [安全工程师](engineering/engineering-security-engineer.md) | 威胁建模、安全代码审查、安全架构 | 应用安全、漏洞评估、安全 CI/CD |

### 🎨 设计部门

让产品美观、易用、令人愉悦。

| 代理 | 专业领域 | 适用场景 |
|-------|-----------|-------------|
| 🎯 [UI 设计师](design/design-ui-designer.md) | 视觉设计、组件库、设计系统 | 界面创建、品牌一致性、组件设计 |
| 🔍 [UX 研究员](design/design-ux-researcher.md) | 用户测试、行为分析、研究 | 理解用户、可用性测试、设计洞察 |
| 🏛️ [UX 架构师](design/design-ux-architect.md) | 技术架构、CSS 系统、实施 | 对开发者友好的基础、实施指导 |
| 🎭 [品牌守护者](design/design-brand-guardian.md) | 品牌身份、一致性、定位 | 品牌战略、身份开发、品牌指南 |
| 📖 [视觉叙事专家](design/design-visual-storyteller.md) | 视觉叙事、多媒体内容 | 引人入胜的视觉故事、品牌叙事 |
| ✨ [趣味注入师](design/design-whimsy-injector.md) | 个性、愉悦感、趣味交互 | 增添乐趣、微交互、彩蛋、品牌个性 |
| 📷 [图像提示词工程师](design/design-image-prompt-engineer.md) | AI 图像生成提示词、摄影 | Midjourney、DALL-E、Stable Diffusion 摄影提示词 |

### 📢 营销部门

一次真诚互动，增长一位受众。

| 代理 | 专业领域 | 适用场景 |
|-------|-----------|-------------|
| 🚀 [增长黑客](marketing/marketing-growth-hacker.md) | 快速用户获取、病毒式传播循环、实验 | 爆发式增长、用户获取、转化优化 |
| 📝 [内容创作者](marketing/marketing-content-creator.md) | 多平台内容、编辑日历 | 内容战略、文案撰写、品牌叙事 |
| 🐦 [Twitter 互动专家](marketing/marketing-twitter-engager.md) | 实时互动、思想领导力 | Twitter 战略、LinkedIn 活动、专业社交 |
| 📱 [TikTok 策略师](marketing/marketing-tiktok-strategist.md) | 病毒式内容、算法优化 | TikTok 增长、病毒式内容、Z 世代/千禧一代受众 |
| 📸 [Instagram 策展人](marketing/marketing-instagram-curator.md) | 视觉叙事、社区建设 | Instagram 战略、美学开发、视觉内容 |
| 🤝 [Reddit 社区建设者](marketing/marketing-reddit-community-builder.md) | 真诚互动、价值驱动内容 | Reddit 战略、社区信任、真实营销 |
| 📱 [应用商店优化师](marketing/marketing-app-store-optimizer.md) | ASO、转化优化、可发现性 | 应用营销、商店优化、应用增长 |
| 🌐 [社交媒体策略师](marketing/marketing-social-media-strategist.md) | 跨平台战略、活动策划 | 整体社交战略、多平台活动 |
| 📕 [小红书运营专家](marketing/marketing-xiaohongshu-specialist.md) | 生活方式内容、趋势驱动策略 | 小红书增长、美学叙事、Z 世代受众 |
| 💬 [微信公众号运营专家](marketing/marketing-wechat-official-account.md) | 订阅者互动、内容营销 | 微信公众号战略、社区建设、转化优化 |
| 🧠 [知乎策略师](marketing/marketing-zhihu-strategist.md) | 思想领导力、知识驱动互动 | 知乎权威建设、问答策略、线索获取 |

### 📊 产品部门

在正确的时间构建正确的产品。

| 代理 | 专业领域 | 适用场景 |
|-------|-----------|-------------|
| 🎯 [Sprint 优先级排序师](product/product-sprint-prioritizer.md) | 敏捷规划、功能优先级 | Sprint 规划、资源分配、待办事项管理 |
| 🔍 [趋势研究员](product/product-trend-researcher.md) | 市场情报、竞争分析 | 市场研究、机会评估、趋势识别 |
| 💬 [反馈综合师](product/product-feedback-synthesizer.md) | 用户反馈分析、洞察提取 | 反馈分析��用户洞察、产品优先级 |

### 🎬 项目管理部门

确保项目按时（且在预算内）完成。

| 代理 | 专业领域 | 适用场景 |
|-------|-----------|-------------|
| 🎬 [工作室制作人](project-management/project-management-studio-producer.md) | 高层协调、组合管理 | 多项目监督、战略对齐、资源分配 |
| 🐑 [项目守护者](project-management/project-management-project-shepherd.md) | 跨职能协调、时间线管理 | 端到端项目协调、利益相关者管理 |
| ⚙️ [工作室运营专家](project-management/project-management-studio-operations.md) | 日常效率、流程优化 | 运营卓越、团队支持、生产力提升 |
| 🧪 [实验追踪师](project-management/project-management-experiment-tracker.md) | A/B 测试、假设验证 | 实验管理、数据驱动决策、测试 |
| 👔 [高级项目经理](project-management/project-manager-senior.md) | 现实范围评估、任务转换 | 将规格转化为任务、范围管理 |

### 🧪 测试部门

替用户发现问题，让他们不必自己遇到。

| 代理 | 专业领域 | 适用场景 |
|-------|-----------|-------------|
| 📸 [证据收集师](testing/testing-evidence-collector.md) | 基于截图的 QA、视觉证明 | UI 测试、视觉验证、Bug 文档 |
| 🔍 [现实核查员](testing/testing-reality-checker.md) | 基于证据的认证、质量关卡 | 生产就绪、质量审批、发布认证 |
| 📊 [测试结果分析师](testing/testing-test-results-analyzer.md) | 测试评估、指标分析 | 测试输出分析、质量洞察、覆盖率报告 |
| ⚡ [性能基准测试师](testing/testing-performance-benchmarker.md) | 性能测试、优化 | 速度测试、负载测试、性能调优 |
| 🔌 [API 测试师](testing/testing-api-tester.md) | API 验证、集成测试 | API 测试、端点验证、集成 QA |
| 🛠️ [工具评估师](testing/testing-tool-evaluator.md) | 技术评估、工具选择 | 评估工具、软件推荐、技术决策 |
| 🔄 [工作流程优化师](testing/testing-workflow-optimizer.md) | 流程分析、工作流程改进 | 流程优化、效率提升、自动化机会 |
| ♿ [无障碍审计师](testing/testing-accessibility-auditor.md) | WCAG 审计、辅助技术测试 | 无障碍合规、屏幕阅读器测试、包容性设计验证 |

### 🛟 支持部门

运营的中坚力量。

| 代理 | 专业领域 | 适用场景 |
|-------|-----------|-------------|
| 💬 [支持响应师](support/support-support-responder.md) | 客户服务、问题解决 | 客户支持、用户体验、支持运营 |
| 📊 [分析报告师](support/support-analytics-reporter.md) | 数据分析、仪表板、洞察 | 商业智能、KPI 追踪、数据可视化 |
| 💰 [财务追踪师](support/support-finance-tracker.md) | 财务规划、预算管理 | 财务分析、现金流、业务绩效 |
| 🏗️ [基础设施维护师](support/support-infrastructure-maintainer.md) | 系统可靠性、性能优化 | 基础设施管理、系统运维、监控 |
| ⚖️ [法务合规检查师](support/support-legal-compliance-checker.md) | 合规、法规、法律审查 | 法律合规、监管要求、风险管理 |
| 📑 [执行摘要生成师](support/support-executive-summary-generator.md) | 高管沟通、战略摘要 | 高管报告、战略沟通、决策支持 |

### 🥽 空间计算部门

构建沉浸式未来。

| 代理 | 专业领域 | 适用场景 |
|-------|-----------|-------------|
| 🏗️ [XR 界面架构师](spatial-computing/xr-interface-architect.md) | 空间交互设计、沉浸式 UX | AR/VR/XR 界面设计、空间计算 UX |
| 💻 [macOS 空间/Metal 工程师](spatial-computing/macos-spatial-metal-engineer.md) | Swift、Metal、高性能 3D | macOS 空间计算、Vision Pro 原生应用 |
| 🌐 [XR 沉浸式开发工程师](spatial-computing/xr-immersive-developer.md) | WebXR、基于浏览器的 AR/VR | 基于浏览器的沉浸式体验、WebXR 应用 |
| 🎮 [XR 座舱交互专家](spatial-computing/xr-cockpit-interaction-specialist.md) | 座舱式控制、沉浸式系统 | 座舱控制系统、沉浸式控制界面 |
| 🍎 [visionOS 空间工程师](spatial-computing/visionos-spatial-engineer.md) | Apple Vision Pro 开发 | Vision Pro 应用、空间计算体验 |
| 🔌 [终端集成专家](spatial-computing/terminal-integration-specialist.md) | 终端集成、命令行工具 | CLI 工具、终端工作流程、开发者工具 |

### 🎯 专项部门

无法被归类的独特专家。

| 代理 | 专业领域 | 适用场景 |
|-------|-----------|-------------|
| 🎭 [代理协调师](specialized/agents-orchestrator.md) | 多代理协调、工作流程管理 | 需要多代理协调的复杂项目 |
| 📊 [数据分析报告师](specialized/data-analytics-reporter.md) | 商业智能、数据洞察 | 深度数据分析、业务指标、战略洞察 |
| 🔍 [LSP/索引工程师](specialized/lsp-index-engineer.md) | Language Server Protocol、代码智能 | 代码智能系统、LSP 实现、语义索引 |
| 📥 [销售数据提取代理](specialized/sales-data-extraction-agent.md) | Excel 监控、销售指标提取 | 销售数据采集、MTD/YTD/年终指标 |
| 📈 [数据整合代理](specialized/data-consolidation-agent.md) | 销售数据聚合、仪表板报告 | 区域汇总、代表绩效、管道快照 |
| 📬 [报告分发代理](specialized/report-distribution-agent.md) | 自动化报告交付 | 基于区域的报告分发、定时发送 |
| 🔐 [代理身份与信任架构师](specialized/agentic-identity-trust.md) | 代理身份、认证、信任验证 | 多代理身份系统、代理授权、审计追踪 |

---

## 🎯 真实世界用例

### 场景一：构建初创公司 MVP

**您的团队**：
1. 🎨 **前端开发工程师** —— 构建 React 应用
2. 🏗️ **后端架构师** —— 设计 API 和数据库
3. 🚀 **增长黑客** —— 规划用户获取
4. ⚡ **快速原型开发工程师** —— 快速迭代周期
5. 🔍 **现实核查员** —— 确保发布前质量

**结果**：在每个阶段都有专业知识的支持，更快交付。

---

### 场景二：营销活动发布

**您的团队**：
1. 📝 **内容创作者** —— 开发活动内容
2. 🐦 **Twitter 互动专家** —— Twitter 战略和执行
3. 📸 **Instagram 策展人** —— 视觉内容和故事
4. 🤝 **Reddit 社区建设者** —— 真诚的社区互动
5. 📊 **分析报告师** —— 追踪和优化绩效

**结果**：具有平台特定专业知识的多渠道协调活动。

---

### 场景三：企业级功能开发

**您的团队**：
1. 👔 **高级项目经理** —— 范围和任务规划
2. 💎 **高级开发工程师** —— 复杂实现
3. 🎨 **UI 设计师** —— 设计系统和组件
4. 🧪 **实验追踪师** —— A/B 测试规划
5. 📸 **证据收集师** —— 质量验证
6. 🔍 **现实核查员** —— 生产就绪检查

**结果**：具有质量关卡和文档的企业级交付���

---

### 场景四：全代理产品发现

**您的团队**：所有 8 个部门同时为一个目标工作。

参见 **[Nexus 空间发现演练](examples/nexus-spatial-discovery.md)** —— 一个完整示例，部署了 8 个代理（产品趋势研究员、后端架构师、品牌守护者、增长黑客、支持响应师、UX 研究员、项目守护者和 XR 界面架构师）同时评估一个软件机会，并产出一个统一的产品计划，涵盖市场验证、技术架构、品牌战略、上市策略、支持系统、UX 研究、项目执行和空间 UI 设计。

**结果**：在单次会话中产出全面、跨职能的产品蓝图。[更多示例](examples/)。

---

## 🤝 贡献

我们欢迎贡献！以下是您可以提供帮助的方式：

### 添加新代理

1. Fork 本仓库
2. 在适当的类别中创建新代理文件
3. 遵循代理模板结构：
   - 包含 name、description、color 的 Frontmatter
   - 身份与记忆章节
   - 核心使命
   - 关键规则（领域特定）
   - 带示例的技术交付成果
   - 工作流程
   - 成功指标
4. 提交包含您代理的 PR

### 改进现有代理

- 添加真实世界示例
- 增强代码示例
- 更新成功指标
- 改进工作流程

### 分享您的成功故事

您是否成功使用了这些代理？在 [讨论区](https://github.com/msitarzewski/agency-agents/discussions) 分享您的故事！

---

## 📖 代理设计理念

每个代理的设计包含：

1. **🎭 强烈个性**：不是通用模板 —— 真实的性格和声音
2. **📋 清晰交付成果**：具体输出，而非模糊指导
3. **✅ 成功指标**：可衡量的结果和质量标准
4. **🔄 经过验证的工作流程**：行之有效的分步流程
5. **💡 学习记忆**：模式识别和持续改进

---

## 🎨 有什么特别之处？

### 与通用 AI 提示不同：
- ❌ 通用"扮演开发者"提示
- ✅ 带有个性化和流程的深度专业化

### 与提示库不同：
- ❌ 一次性提示集合
- ✅ 包含工作流程和交付成果的全面代理系统

### 与 AI 工具不同：
- ❌ 无法自定义的黑盒工具
- ✅ 透明、可分支、可适配的代理人格

---

## 🎨 代理个性亮点

> "我不只是测试你的代码 —— 我默认会找出 3-5 个问题，并要求一切都有视觉证明。"
>
> —— **证据收集师**（测试部门）

> "你不是在 Reddit 上做营销 —— 你是在成为一个恰好代表一个品牌的受重视的社区成员。"
>
> —— **Reddit 社区建设者**（营销部门）

> "每个趣味元素都必须服务于功能性或情感目的。设计的是增强而非分散注意力的愉悦感。"
>
> —— **趣味注入师**（设计部门）

> "让我添加一个庆祝动画，可以将任务完成焦虑降低 40%"
>
> —— **趣味注入师**（在 UX 审查期间）

---

## 📊 统计数据

- 🎭 **61 个专业代理** 分布在 9 个部门
- 📝 **10,000+ 行** 个性、流程和代码示例
- ⏱️ **数月迭代** 源于真实世界使用
- 🌟 **经实战检验** 在生产环境中
- 💬 **50+ 请求** 在 Reddit 上发布的头 12 小时内

---

## 🔌 多工具集成

The Agency 原生支持 Claude Code，并提供转换 + 安装脚本，让您可以在所有主流智能编程工具中使用相同的代理。

### 支持的工具

- **[Claude Code](https://claude.ai/code)** —— 原生 `.md` 代理，无需转换 → `~/.claude/agents/`
- **[Antigravity](https://github.com/google-gemini/antigravity)** —— 每个代理一个 `SKILL.md` → `~/.gemini/antigravity/skills/`
- **[Gemini CLI](https://github.com/google-gemini/gemini-cli)** —— 扩展 + `SKILL.md` 文件 → `~/.gemini/extensions/agency-agents/`
- **[OpenCode](https://opencode.ai)** —— `.md` 代理文件 → `.opencode/agent/`
- **[Cursor](https://cursor.sh)** —— `.mdc` 规则文件 → `.cursor/rules/`
- **[Aider](https://aider.chat)** —— 单个 `CONVENTIONS.md` → `./CONVENTIONS.md`
- **[Windsurf](https://codeium.com/windsurf)** —— 单个 `.windsurfrules` → `./.windsurfrules`

---

### ⚡ 快速安装

**步骤一 —— 生成集成文件：**
```bash
./scripts/convert.sh
```

**步骤二 —— 安装（交互式，自动检测您的工具）：**
```bash
./scripts/install.sh
```

安装程序会扫描您系统上已安装的工具，显示复选框界面，让您精确选择要安装的内容：

```
  +------------------------------------------------+
  |   The Agency -- 工具安装程序                    |
  +------------------------------------------------+

  系统扫描: [*] = 在此机器上检测到

  [x]  1)  [*]  Claude Code     (claude.ai/code)
  [x]  2)  [*]  Antigravity     (~/.gemini/antigravity)
  [ ]  3)  [ ]  Gemini CLI      (gemini extension)
  [ ]  4)  [ ]  OpenCode        (opencode.ai)
  [x]  5)  [*]  Cursor          (.cursor/rules)
  [ ]  6)  [ ]  Aider           (CONVENTIONS.md)
  [ ]  7)  [ ]  Windsurf        (.windsurfrules)

  [1-7] 切换   [a] 全选   [n] 全不选   [d] 已检测
  [Enter] 安装   [q] 退出
```

**或直接安装特定工具：**
```bash
./scripts/install.sh --tool cursor
./scripts/install.sh --tool opencode
./scripts/install.sh --tool antigravity
```

**非交互式（CI/脚本）：**
```bash
./scripts/install.sh --no-interactive --tool all
```

---

### 特定工具说明

<details>
<summary><strong>Claude Code</strong></summary>

代理直接从仓库复制到 `~/.claude/agents/` —— 无需转换。

```bash
./scripts/install.sh --tool claude-code
```

然后在 Claude Code 中激活：
```
Use the Frontend Developer agent to review this component.
```

详见 [integrations/claude-code/README.md](integrations/claude-code/README.md)。
</details>

<details>
<summary><strong>Antigravity (Gemini)</strong></summary>

每个代理变成 `~/.gemini/antigravity/skills/agency-<slug>/` 中的技能。

```bash
./scripts/install.sh --tool antigravity
```

在 Gemini with Antigravity 中激活：
```
@agency-frontend-developer review this React component
```

详见 [integrations/antigravity/README.md](integrations/antigravity/README.md)。
</details>

<details>
<summary><strong>Gemini CLI</strong></summary>

作为 Gemini CLI 扩展安装，包含 61 个技能 + 一个清单。

```bash
./scripts/install.sh --tool gemini-cli
```

详见 [integrations/gemini-cli/README.md](integrations/gemini-cli/README.md)。
</details>

<details>
<summary><strong>OpenCode</strong></summary>

代理放置在项目根目录的 `.opencode/agent/` 中（项目范围）。

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool opencode
```

或全局安装：
```bash
mkdir -p ~/.config/opencode/agent
cp integrations/opencode/agent/*.md ~/.config/opencode/agent/
```

在 OpenCode 中激活：
```
Use the Backend Architect agent to design this API.
```

详见 [integrations/opencode/README.md](integrations/opencode/README.md)。
</details>

<details>
<summary><strong>Cursor</strong></summary>

每个代理变成项目 `.cursor/rules/` 中的 `.mdc` 规则文件。

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool cursor
```

当 Cursor 检测到规则时会自动应用。显式引用：
```
Use the @security-engineer rules to review this code.
```

详见 [integrations/cursor/README.md](integrations/cursor/README.md)。
</details>

<details>
<summary><strong>Aider</strong></summary>

所有代理编译成单个 `CONVENTIONS.md` 文件，Aider 会自动读取。

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool aider
```

然后在 Aider 会话中引用代理：
```
Use the Frontend Developer agent to refactor this component.
```

详见 [integrations/aider/README.md](integrations/aider/README.md)。
</details>

<details>
<summary><strong>Windsurf</strong></summary>

所有代理编译成项目根目录的 `.windsurfrules`。

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool windsurf
```

在 Windsurf 的 Cascade 中引用代理：
```
Use the Reality Checker agent to verify this is production ready.
```

详见 [integrations/windsurf/README.md](integrations/windsurf/README.md)。
</details>

---

### 更改后重新生成

当您添加新代理或编辑现有代理时，重新生成所有集成文件：

```bash
./scripts/convert.sh        # 重新生成所有
./scripts/convert.sh --tool cursor   # 只重新生成一个工具
```

---

## 🗺️ 路线图

- [ ] 交互式代理选择器 Web 工具
- [x] 多代理工作流程示例 —— 见 [examples/](examples/)
- [x] 多工具集成脚本（Claude Code、Antigravity、Gemini CLI、OpenCode、Cursor、Aider、Windsurf）
- [ ] 代理设计视频教程
- [ ] 社区代理市场
- [ ] 代理"人格测验"用于项目匹配
- [ ] "每周代理"展示系列

---

## 🌐 社区翻译与本地化

社区维护的翻译和区域适配版本。这些由独立维护 —— 请查看各仓库了解覆盖范围和版本兼容性。

| 语言 | 维护者 | 链接 | 备注 |
|----------|-----------|------|-------|
| 🇨🇳 简体中文 (zh-CN) | [@jnMetaCode](https://github.com/jnMetaCode) | [agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh) | 26 个翻译代理 + 4 个中国市场代理 |

想添加翻译？提交一个 issue，我们会在这里链接。

---

## 📜 许可证

MIT License - 可自由用于商业或个人用途。感谢注明出处，但不作强制要求。

---

## 🙏 致谢

源于一次关于 AI 代理专业化的 Reddit 讨论。感谢社区的反馈、请求和灵感。

特别感谢在头 12 小时内提出请求的 50 多位 Reddit 用户 —— 你们证明了市场对真正专业化的 AI 代理系统的需求。

---

## 💬 社区

- **GitHub Discussions**: [分享您的成功故事](https://github.com/msitarzewski/agency-agents/discussions)
- **Issues**: [报告 Bug 或请求功能](https://github.com/msitarzewski/agency-agents/issues)
- **Reddit**: 在 r/ClaudeAI 参与讨论
- **Twitter/X**: 使用 #TheAgency 分享

---

## 🚀 开始使用

1. **浏览** 上方的代理列表，找到适合您需求的专家
2. **复制** 代理到 `~/.claude/agents/` 以进行 Claude Code 集成
3. **激活** 代理，在您的 Claude 对话中引用它们
4. **自定义** 代理人格和工作流程以适应您的特定需求
5. **分享** 您的结果并向社区回馈

---

<div align="center">

**🎭 The Agency：您的 AI 梦之队正在等待 🎭**

[⭐ 给仓库加星](https://github.com/msitarzewski/agency-agents) • [🍴 Fork 它](https://github.com/msitarzewski/agency-agents/fork) • [🐛 报告问题](https://github.com/msitarzewski/agency-agents/issues) • [❤️ 赞助](https://github.com/sponsors/msitarzewski)

用 ❤️ 由社区制作，为社区服务

</div>