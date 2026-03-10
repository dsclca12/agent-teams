# Claude Code 集成

The Agency 是为 Claude Code 构建的。无需转换 — 智能体以现有的 `.md` + YAML frontmatter 格式原生工作。

## 安装

```bash
# 将所有智能体复制到您的 Claude Code 智能体目录
./scripts/install.sh --tool claude-code

# 或手动复制某个类别
cp engineering/*.md ~/.claude/agents/
```

## 激活智能体

在任何 Claude Code 会话中，通过名称引用智能体：

```
Activate Frontend Developer and help me build a React component.
```

```
Use the Reality Checker agent to verify this feature is production-ready.
```

## 智能体目录

智能体按部门组织。完整 61 位专家名单请参阅 [主 README](../../README.md)。