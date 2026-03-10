# Cursor 集成

将所有 61 个 Agency 智能体转换为 Cursor `.mdc` 规则文件。规则是**项目级别的** — 请从项目根目录安装。

## 安装

```bash
# 从项目根目录运行
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool cursor
```

这将在您的项目中创建 `.cursor/rules/<agent-slug>.mdc` 文件。

## 激活规则

在 Cursor 中，在提示中引用智能体：

```
@frontend-developer Review this React component for performance issues.
```

或通过编辑 frontmatter 将规则设置为始终启用：

```yaml
---
description: Expert frontend developer...
globs: "**/*.tsx,**/*.ts"
alwaysApply: true
---
```

## 重新生成

```bash
./scripts/convert.sh --tool cursor
```