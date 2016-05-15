# 安装 Chrome 浏览器

Chrome 已经成为除 IE 以外，市场占有率最高，跨平台，“开发人员必备的”浏览器，所以是未来网页浏览和 Web 开发的必备工具。

## 命令行安装（推荐）

```bash
wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
```

```bash
sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" > /etc/apt/sources.list.d/google.list'
```

```bash
sudo apt update
sudo apt install google-chrome-stable
```

## 或者使用安装包安装（二选一）

- [百度网盘下载](http://pan.baidu.com/s/1eQS7c8E)（不需要翻墙，需要安装后更新至最新版本）
- [官网下载](https://www.google.com/chrome/)（最新版本，可能需要翻墙）
