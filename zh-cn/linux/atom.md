# 安装 Atom 文本编辑器

## Linux Mint & Ubuntu & Deepin

```bash
$ sudo add-apt-repository ppa:webupd8team/atom
$ sudo apt-get update
$ sudo apt-get install atom
```

### 安装 Atom 的扩展包

```bash
$ apm install linter linter-jshint editorconfig atom-beautify
```

### 设置支持中文的等宽字体（推荐，可根据个人喜好调整）

菜单路径：`Edit` -> `Preferences` -> `Settings` -> `Editor Settings` -> `Font Family`

填入字体名（文泉驿等宽微米黑）：`WenQuanYi Micro Hei Mono`

### 设置显示格式

菜单路径：`Edit` -> `Preferences` -> `Settings` -> `Editor Settings`

将 `Show Indent Guide（用于显示缩进参考线）` 和 `Show Invisibles（用于显示费非可见内容，比如空格和Tab）` 两项勾选开启。
