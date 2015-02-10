# 安装 Chrome 浏览器

## Linux Mint & Ubuntu

### 安装 Google Linux Repository 密钥

```bash
$ wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
```

### 添加 Google Chrome 软件源信息

```bash
$ sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'
```

### 更新软件源信息并安装 Chrome 浏览器

```bash
$ sudo apt-get update
$ sudo apt-get install google-chrome-stable
```
