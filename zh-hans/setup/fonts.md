# 优化中文显示

## 安装新字体

Ubuntu 本身所带的字体十分有限，不能很好的满足日常的显示和文字编辑工作，所以如果想要使用更多的字体，可以将 Windows 系统的全部字体文件拷贝至用户 Home 目录下名为 `.fonts` 的文件夹下（需要手动创建，`.fonts` 在创建后是隐藏文件夹，可以在文件浏览窗口中按快捷键 Ctrl + H 显示出来）。

## 优化中文显示

### 优化系统默认字体配置

0. 下载字体配置文件：[百度网盘下载](http://pan.baidu.com/s/1kU6blcj)
0. 将下载的 .fonts.conf 文件放置在 Home 目录下，注意，使用 Firefox 下载该文件会导致该文件被重命名为 fonts.conf，我们需要将其重新改为 .fonts.conf（ .fonts.conf 是一个隐藏文件，可以在文件浏览窗口中按快捷键 Ctrl + H 显示出来）。

### 优化浏览器默认显示字体

#### Firefox

0. 在 Firefox 菜单的 Edit 中打开 Preferences 设置界面
0. 然后在 Content 选项卡中点击 Advanced 按钮打开 Fonts 高级设置
0. 在弹出的窗口中，将 Fonts for 修改为 Simplified Chinese
0. 点击 OK 按钮完成设置。

#### Chrome

0. 在 Chrome 菜单的 Edit 中打开 Preferences 设置界面
0. 然后在 Settings 选项卡中将页面拖至最下方点击 Show advanced settings... 展开高级设置
0. 在展开后的内容中找到 Web content 部分，点击 Customize fonts... 按钮打开字体和编码设置
0. 将 Standard font 修改为 Sans
0. 将 Serif font 修改为 Serif
0. 将 Sans-serif font 修改为 Sans
0. 确保 Fixed-width font 选择为 Monospace
0. 点击 Done 按钮完成设置。
