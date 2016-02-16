# 安装 Chrome 浏览器

Chrome 已经成为除 IE 以外，市场占有率最高，跨平台，“开发人员必备的”浏览器，所以是未来网页浏览和 Web 开发的必备工具。

## 方法一：安装包安装（二选一）

- [百度网盘下载](http://pan.baidu.com/s/1eRdSXxC)（不需要翻墙，需要安装后更新至最新版本）
- [官网下载](https://www.google.com/chrome/)（最新版本，可能需要翻墙）

## 方法二：命令行安装（可能需要翻墙）

### 安装 Google Linux Repository 密钥

```bash
$ wget -q -O - https://dl-ssl.google.com/setup/linux_signing_key.pub | sudo apt-key add -
```

### 添加 Google Chrome 软件源信息

```bash
$ sudo sh -c 'echo "deb http://dl.google.com/setup/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'
```

### 更新软件源信息并安装 Chrome 浏览器

```bash
$ sudo apt-get update
$ sudo apt-get install google-chrome-stable
```
