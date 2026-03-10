# Aider 集成

所有 61 个 Agency 智能体合并为一个 `CONVENTIONS.md` 文件。当该文件存在于项目根目录时，Aider 会自动读取。

## 安装

```bash
# 从项目根目录运行
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool aider
```

## 激活智能体

在 Aider 会话中，通过名称引用智能体：

```
Use the Frontend Developer agent to refactor this component.
```

```
Apply the Reality Checker agent to verify this is production-ready.
```

## 手动使用

您也可以直接传递规范文件：

```bash
aider --read CONVENTIONS.md
```

## 重新生成

```bash
./scripts/convert.sh --tool aider
```