# Windsurf 集成

所有 61 个 Agency 智能体合并为一个 `.windsurfrules` 文件。规则是**项目级别的** — 请从项目根目录安装。

## 安装

```bash
# 从项目根目录运行
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool windsurf
```

## 激活智能体

在 Windsurf 中，在提示中通过名称引用智能体：

```
Use the Frontend Developer agent to build this component.
```

## 重新生成

```bash
./scripts/convert.sh --tool windsurf
```