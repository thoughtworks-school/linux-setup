# 安装常用字体并优化中文显示

Ubuntu 本身所带的字体十分有限，不能很好的满足日常的显示和文字编辑工作，所以我已准备好以下字体来予以改进：

- 全部的 Windows 字体（满足日常文字编辑、文档及网页显示需要）

## 下载并安装字体

### 下载

- [Windows 字体文件压缩包](http://pan.baidu.com/s/1o85shPg)

### 安装

将下载的 `ms-fonts.tar.gz` 压缩包中的全部文件解压，将解压后得到的内容剪切 `Ctrl + X` 并粘贴 `Ctrl + V` 至（如果是使用复制粘贴，可能会造成 Ubuntu 卡住，不过不用担心，等待完成就好）文件浏览器 Home 目录下名为 `.fonts` 的文件夹下（需要手动创建，`.fonts` 在创建后是隐藏文件夹，可以在文件浏览窗口中按快捷键 Ctrl + H 显示出来）。

## 优化中文显示

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
0. 点击 OK 按钮完成设置。
