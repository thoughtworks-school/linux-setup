# 安装 Visual Studio Code 文本编辑器

Visual Studio Code 是由微软公司基于 Atom 文本编辑器开发的一款强大的开源、跨平台文本编辑器，可以在不需要 IDE 的场合进行轻量级开发和文本编辑。

添加官方包管理器源信息：

```bash
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg
sudo sh -c 'echo "deb [arch=amd64] http://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'
```

安装 Visual Studio Code

```bash
sudo apt update
sudo apt install code
```