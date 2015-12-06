# 安装 Chrome 浏览器

## Linux Mint & Ubuntu

### 安装包安装（需要翻墙）

[官网下载](https://www.google.com/chrome/)

### 命令行安装（需要翻墙）

#### 安装 Google Linux Repository 密钥

```bash
$ wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
```

#### 添加 Google Chrome 软件源信息

```bash
$ sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'
```

#### 更新软件源信息并安装 Chrome 浏览器

```bash
$ sudo apt-get update
$ sudo apt-get install google-chrome-stable
```

## Deepin

已预置，但版本更新相对滞后一点，如需要保持版本最新，请参考上方的安装方法。
