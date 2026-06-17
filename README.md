# shuiye-ui

<!-- skillgit:start -->
> 这是 Codex skill **shuiye-ui** 的远程仓库，由 `shuiye-skillgit` 管理展示内容。

## 用途

分析开发任务和产品需求，设计页面结构与交互流程，生成、修改和预览可操作的 HTML/CSS/JavaScript 原型。当用户需要创建 UI 原型、调整已有页面、检查原型环境或启动本地预览时使用。

## 调用方式

```text
$shuiye-ui
$shuiye-ui edit <页面或文件> <修改需求>
$shuiye-ui env
$shuiye-ui preview [端口]
$shuiye-ui help
$shuiye-ui upgrade <优化想法>
```

## Skill 结构

```text
shuiye-ui/
├── SKILL.md
├── agents/ (1 file)
├── references/ (2 files)
└── assets/ (1 file)
```

## 安装

远程仓库包含展示用 `README.md`，安装到 Codex 时不复制该文件：

```bash
tmp_dir="$(mktemp -d)"
git clone git@github.com:shuiye-skills/shuiye-ui.git "$tmp_dir/shuiye-ui"
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills/shuiye-ui"
rsync -a --exclude='.git/' --exclude='README.md' \
  "$tmp_dir/shuiye-ui/" \
  "${CODEX_HOME:-$HOME/.codex}/skills/shuiye-ui/"
rm -rf "$tmp_dir"
```

安装后入口位于：

```text
${CODEX_HOME:-$HOME/.codex}/skills/shuiye-ui/SKILL.md
```
<!-- skillgit:end -->
