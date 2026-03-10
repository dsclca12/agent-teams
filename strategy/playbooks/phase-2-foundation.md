# ⚙️ Phase 2 Playbook —— 基础与脚手架

> **持续时间**：3-5 天 | **Agent 数量**：6 | **门控负责人**：DevOps Automator + Evidence Collector

---

## 目标

构建所有后续工作依赖的技术和运营基础。在添加肌肉之前让骨架先站立起来。此阶段后，每个开发者都有一个可工作的环境、一个可部署的流水线和一个可用的设计系统。

## 前置条件

- [ ] Phase 1 质量门控通过（架构包已批准）
- [ ] Phase 1 交接包已接收
- [ ] 所有架构文档已最终确定

## Agent 激活序列

### 工作流 A：基础设施（第 1-3 天，并行）

#### 🚀 DevOps Automator —— CI/CD 流水线 + 基础设施
```
激活 DevOps Automator 为 [项目] 设置基础设施。

输入：Backend Architect 系统架构 + 部署要求
所需交付物：
1. CI/CD 流水线（GitHub Actions / GitLab CI）
   - 安全扫描阶段
   - 自动化测试阶段
   - 构建和容器化阶段
   - 部署阶段（蓝绿或金丝雀）
   - 自动回滚能力
2. 基础设施即代码
   - 环境配置（开发、预发布、生产）
   - 容器编排设置
   - 网络和安全配置
3. 环境配置
   - 密钥管理
   - 环境变量管理
   - 多环境一致性

要创建的文件：
- .github/workflows/ci-cd.yml（或等效文件）
- infrastructure/（Terraform/CDK 模板）
- docker-compose.yml
- Dockerfile(s)

格式：可工作的 CI/CD 流水线及 IaC 模板
时间线：3 天
```

#### 🏗️ Infrastructure Maintainer —— 云基础设施 + 监控
```
激活 Infrastructure Maintainer 为 [项目] 设置监控。

输入：DevOps Automator 基础设施 + Backend Architect 架构
所需交付物：
1. 云资源配置
   - 计算、存储、网络资源
   - 自动扩缩容配置
   - 负载均衡器设置
2. 监控栈
   - 应用指标（Prometheus/DataDog）
   - 基础设施指标
   - 自定义仪表板（Grafana）
3. 日志和告警
   - 集中式日志聚合
   - 关键阈值的告警规则
   - 值班通知设置
4. 安全加固
   - 防火墙规则
   - SSL/TLS 配置
   - 访问控制策略

格式：带仪表板访问权限的基础设施就绪报告
时间线：3 天
```

#### ⚙️ Studio Operations —— 流程设置
```
激活 Studio Operations 为 [项目] 设置流程。

输入：Sprint Prioritizer 计划 + Project Shepherd 协调需求
所需交付物：
1. Git 工作流
   - 分支策略（GitFlow / 主干开发）
   - PR 审查流程
   - 合并策略
2. 沟通渠道
   - 团队频道设置
   - 通知路由
   - 状态更新节奏
3. 文档模板
   - PR 模板
   - Issue 模板
   - 决策日志模板
4. 协作工具
   - 项目看板设置
   - 冲刺跟踪配置

格式：运营 Playbook
时间线：2 天
```

### 工作流 B：应用基础（第 1-4 天，并行）

#### 🎨 Frontend Developer —— 项目脚手架 + 组件库
```
激活 Frontend Developer 为 [项目] 进行项目脚手架搭建。

输入：UX Architect CSS 设计系统 + Brand Guardian 标识
所需交付物：
1. 项目脚手架
   - 框架设置（按架构的 React/Vue/Angular）
   - TypeScript 配置
   - 构建工具（Vite/Webpack/Next.js）
   - 测试框架（Jest/Vitest + Testing Library）
2. 设计系统实现
   - 来自 UX Architect 的 CSS 设计令牌
   - 基础组件库（Button、Input、Card、Layout）
   - 主题系统（浅色/深色/系统切换）
   - 响应式工具
3. 应用外壳
   - 路由设置
   - 布局组件（Header、Footer、Sidebar）
   - 错误边界实现
   - 加载状态

要创建的文件：
- src/（应用��代码）
- src/components/（组件库）
- src/styles/（设计令牌）
- src/layouts/（布局组件）

格式：可工作的应用骨架及组件库
时间线：3 天
```

#### 🏗️ Backend Architect —— 数据库 + API 基础
```
激活 Backend Architect 为 [项目] 搭建 API 基础。

输入：系统架构规范 + 数据库 Schema 设计
所需交付物：
1. 数据库设置
   - Schema 部署（迁移）
   - 索引创建
   - 开发用种子数据
   - 连接池配置
2. API 脚手架
   - 框架设置（Express/FastAPI 等）
   - 匹配架构的路由结构
   - 中间件栈（认证、验证、错误处理、CORS）
   - 健康检查端点
3. 认证系统
   - 认证提供商集成
   - JWT/会话管理
   - 基于角色的访问控制脚手架
4. 服务通信
   - API 版本管理设置
   - 请求/响应序列化
   - 错误响应标准化

要创建的文件：
- api/ 或 server/（后端源代码）
- migrations/（数据库迁移）
- docs/api-spec.yaml（OpenAPI 规范）

格式：可工作的 API 脚手架及数据库和认证
时间线：4 天
```

#### 🏛️ UX Architect —— CSS 系统实现
```
激活 UX Architect 为 [项目] 实现 CSS 系统。

输入：Brand Guardian 标识 + 自己的 Phase 1 CSS 设计系统规范
所需交付物：
1. 设计令牌实现
   - CSS 自定义属性（颜色、排版、间距）
   - 带语义命名的品牌色彩调色板
   - 带响应式调整的排版比例
2. 布局系统
   - 容器系统（响应式断点）
   - Grid 模式（2 列、3 列、侧边栏）
   - Flexbox 工具
3. 主题系统
   - 浅色主题变量
   - 深色主题变量
   - 系统偏好检测
   - 主题切换组件
   - 主题间的平滑过渡

要创建/更新的文件：
- css/design-system.css（或框架中的等效文件）
- css/layout.css
- css/components.css
- js/theme-manager.js

格式：已实现的 CSS 设计系统及主题切换
时间线：2 天
```

## 验证检查点（第 4-5 天）

### Evidence Collector 验证
```
激活 Evidence Collector 进行 Phase 2 基础验证。

用截图证据验证以下内容：
1. CI/CD 流水线成功执行（显示流水线日志）
2. 应用骨架在浏览器中加载（桌面截图）
3. 应用骨架在移动端加载（移动端截图）
4. 主题切换工作正常（浅色 + 深色截图）
5. API 健康检查响应（curl 输出）
6. 数据库可访问（迁移状态）
7. 监控仪表板激活（仪表板截图）
8. 组件库渲染正常（组件演示页面）

格式：带截图的证据包
裁决：PASS / FAIL 及具体问题
```

## 质量门控检查清单

| # | 标准 | 证据来源 | 状态 |
|---|------|---------|------|
| 1 | CI/CD 流水线可构建、测试和部署 | 流水线执行日志 | ☐ |
| 2 | 数据库 Schema 已部署及所有表/索引 | 迁移成功输出 | ☐ |
| 3 | API 脚手架在健康检查上响应 | curl 响应证据 | ☐ |
| 4 | 前端骨架在��览器中渲染 | Evidence Collector 截图 | ☐ |
| 5 | 监控仪表板显示指标 | 仪表板截图 | ☐ |
| 6 | 设计系统令牌已实现 | 组件库演示 | ☐ |
| 7 | 主题切换功能正常（浅色/深色/系统） | 前后截图 | ☐ |
| 8 | Git 工作流和流程已文档化 | Studio Operations playbook | ☐ |

## 门控决策

**需要双重签核**：DevOps Automator（基础设施）+ Evidence Collector（视觉）

- **PASS**：可工作的骨架及完整 DevOps 流水线 → Phase 3 激活
- **FAIL**：具体的基础设施或应用问题 → 修复并重新验证

## 交接到 Phase 3

```markdown
## Phase 2 → Phase 3 交接包

### 给所有开发者 Agent：
- 可工作的 CI/CD 流水线（合并时自动部署）
- 设计系统令牌和组件库
- 带认证和健康检查的 API 脚手架
- 带 Schema 和种子数据的数据库
- Git 工作流和 PR 流程

### 给 Evidence Collector（持续 QA）：
- 应用 URL（开发、预发布）
- 截图捕获方法
- 组件库参考
- 视觉验证的品牌指南

### 给 Agents Orchestrator（Dev↔QA 循环管理）：
- Sprint Prioritizer Backlog（来自 Phase 1）
- 带验收标准的任务列表（来自 Phase 1）
- Agent 分配矩阵（来自 NEXUS 策略）
- 每种任务类型的质量阈值

### 环境访问：
- 开发环境：[URL]
- 预发布环境：[URL]
- 监控仪表板：[URL]
- CI/CD 流水线：[URL]
- API 文档：[URL]
```

---

*当骨架应用运行、CI/CD 流水线可操作、Evidence Collector 已用截图验证所有基础元素时，Phase 2 完成。*