# OpenCode 集成

OpenCode 使用与 Claude Code 相同的智能体格式 — 即存储在 `.opencode/agent/` 中带有 YAML frontmatter 的 `.md` 文件。技术上无需转换，但此集成将智能体打包到正确的目录结构中，以便直接使用。

## 安装

```bash
# 从项目根目录运行
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool opencode
```

这将在您的项目目录中创建 `.opencode/agent/<slug>.md` 文件。

## 激活智能体

在 OpenCode 中，通过名称或描述引用智能体：

```
Use the Frontend Developer agent to help build this component.
```

```
Activate the Reality Checker agent and review this PR.
```

您也可以从 OpenCode UI 的智能体选择器中选择智能体。

## 智能体格式

OpenCode 智能体使用与 Claude Code 相同的 frontmatter：

```yaml
---
name: Frontend Developer
description: Expert frontend developer specializing in modern web technologies...
color: cyan
---
```

## 项目级别 vs 全局

`.opencode/agent/` 中的智能体是**项目级别的**。要使其在所有项目中全局可用，请将它们复制到您的 OpenCode 配置目录：

```bash
mkdir -p ~/.config/opencode/agent
cp integrations/opencode/agent/*.md ~/.config/opencode/agent/
```

## 重新生成

```bash
./scripts/convert.sh --tool opencode
```