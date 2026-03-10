# Gemini CLI 集成

将所有 61 个 Agency 智能体打包为 Gemini CLI 扩展。扩展安装到 `~/.gemini/extensions/agency-agents/`。

## 安装

```bash
./scripts/install.sh --tool gemini-cli
```

## 激活技能

在 Gemini CLI 中，通过名称引用智能体：

```
Use the frontend-developer skill to help me build this UI.
```

## 扩展结构

```
~/.gemini/extensions/agency-agents/
  gemini-extension.json
  skills/
    frontend-developer/SKILL.md
    backend-architect/SKILL.md
    reality-checker/SKILL.md
    ...
```

## 重新生成

```bash
./scripts/convert.sh --tool gemini-cli
```