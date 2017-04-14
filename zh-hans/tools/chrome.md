# 安装 Chrome 浏览器（需要翻墙）

Chrome 已经成为除 IE 以外，市场占有率最高，跨平台，“开发人员必备的”浏览器，所以是未来网页浏览和 Web 开发的必备工具，如果你擅长翻墙，请优先安装此版本。

```bash
wget -O ~/Downloads/google-chrome-stable_current_amd64.deb https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i ~/Downloads/google-chrome-stable_current_amd64.deb
sudo apt install -f
```

## 替代品：安装 Chromium 浏览器

Chromium 是 Chrome 的开源版本，主要是没有捆绑一些需要版权的插件，比如 Flash，由于 Ubuntu 软件仓库自带并更新较快，所以在无法翻墙的情况下我们推荐使用 Chromium 代替 Chrome，更多 Chromium 和 Chrome 的关系请见：

https://www.zhihu.com/question/27046250

```bash
sudo apt update
sudo apt install chromium-browser
```