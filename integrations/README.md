# 🔌 集成

本目录包含 The Agency 的 61 个 AI 智能体，已转换为兼容主流智能编程工具的格式。

## 支持的工具

- **[Claude Code](#claude-code)** — `.md` 智能体文件，直接使用本仓库
- **[Antigravity](#antigravity)** — 每个智能体对应 `antigravity/` 目录下的 `SKILL.md` 文件
- **[Gemini CLI](#gemini-cli)** — 扩展 + `gemini-cli/` 目录下的 `SKILL.md` 文件
- **[OpenCode](#opencode)** — `opencode/` 目录下的 `.md` 智能体文件
- **[Cursor](#cursor)** — `cursor/` 目录下的 `.mdc` 规则文件
- **[Aider](#aider)** — `aider/` 目录下的 `CONVENTIONS.md` 文件
- **[Windsurf](#windsurf)** — `windsurf/` 目录下的 `.windsurfrules` 文件

## 快速安装

```bash
# 自动为所有检测到的工具安装
./scripts/install.sh

# 为特定工具安装
./scripts/install.sh --tool antigravity
./scripts/install.sh --tool gemini-cli
./scripts/install.sh --tool cursor
./scripts/install.sh --tool aider
./scripts/install.sh --tool windsurf
./scripts/install.sh --tool claude-code
```

## 重新生成集成文件

如果您添加或修改了智能体，请重新生成所有集成文件：

```bash
./scripts/convert.sh
```

---

## Claude Code

The Agency 最初是为 Claude Code 设计的。智能体无需转换即可原生工作。

```bash
cp -r <category>/*.md ~/.claude/agents/
# 或一次性安装所有智能体：
./scripts/install.sh --tool claude-code
```

详情请参阅 [claude-code/README.md](claude-code/README.md)。

---

## Antigravity

技能安装到 `~/.gemini/antigravity/skills/`。每个智能体变成一个独立的技能，以 `agency-` 为前缀以避免命名冲突。

```bash
./scripts/install.sh --tool antigravity
```

详情请参阅 [antigravity/README.md](antigravity/README.md)。

---

## Gemini CLI

智能体被打包为 Gemini CLI 扩展，包含独立的技能文件。扩展安装到 `~/.gemini/extensions/agency-agents/`。

```bash
./scripts/install.sh --tool gemini-cli
```

详情请参阅 [gemini-cli/README.md](gemini-cli/README.md)。

---

## Cursor

每个智能体变成一个 `.mdc` 规则文件。规则是项目级别的 — 请从项目根目录运行安装程序。

```bash
cd /your/project && /path/to/agency-agents/scripts/install.sh --tool cursor
```

详情请参阅 [cursor/README.md](cursor/README.md)。

---

## Aider

所有智能体合并为一个 `CONVENTIONS.md` 文件，当该文件存在于项目根目录时，Aider 会自动读取。

```bash
cd /your/project && /path/to/agency-agents/scripts/install.sh --tool aider
```

详情请参阅 [aider/README.md](aider/README.md)。

---

## Windsurf

所有智能体合并为一个 `.windsurfrules` 文件，用于项目根目录。

```bash
cd /your/project && /path/to/agency-agents/scripts/install.sh --tool windsurf
```

详情请参阅 [windsurf/README.md](windsurf/README.md)。