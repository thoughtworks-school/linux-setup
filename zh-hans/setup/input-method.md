# 安装中文输入法

经过测试，系统自带的基于 IBus 输入法框架的 Intelligent Pinyin 是目前兼容性最好且最为稳定的中文输入法，只是词库实在是不够智能。

而搜狗输入法 Linux 版则基于 Fcitx 输入法框架，相对以前来有了很大改进，输入体验是目前Linux上最强，但是依然还不是很成熟，目前最大的干扰是搜狗输入法常驻运行，无法完全切换至英文，只能按 Shift 键在中英文间来回切换，比较影响输入（因人而异）。

所以，请根据个人喜好尝试并根据试用结果选择一种输入法。

## IBus 输入法框架 + Intelligent Pinyin 输入法

### Ubuntu

```bash
$ sudo apt-get update
$ sudo apt-get install ibus-libpinyin
```

确认在 Language Support 中将 Keyboard input method system 选择为 IBus 输入法框架。

注销当前用户并重新登录，在 Text Entry 中添加 Intelligent Pinyin 输入法。

成功后按 Windows徽标键 + 空格键 切换中英文输入法。

### Linux Mint

```bash
$ sudo apt-get update
$ sudo apt-get install ibus ibus-libpinyin
```

注销当前用户并重新登录，在 Input Method 中将 Input method 选择为 IBus 输入法框架。

注销当前用户并重新登录，在 Keyboard Input Methods 中添加 Intelligent Pinyin 输入法。

成功后按 Ctrl + 空格键 切换中英文输入法。

## Fcitx 输入法框架 + 搜狗输入法

### Ubuntu

下载64位的搜狗输入法 Linux 版：

[前往官网下载](http://pinyin.sogou.com/linux/)

双击下载下来的 deb 安装文件进行安装。

注销当前用户并重新登录，在 Language Support 中将 Keyboard input method system 选择为 fcitx 输入法框架。

注销当前用户并重新登陆，在 Fcitx Configuration 中添加 Sogou Pinyin 输入法（添加时记得点掉 Only Show Current Language 复选框）。

注销当前用户并重新登陆，按 Ctrl + 空格键 切换中英文输入法（然后搜狗输入法就会常驻，只能按 Shift 键切换中英文）。

### Linux Mint

下载64位的搜狗输入法 Linux 版：

[前往官网下载](http://pinyin.sogou.com/linux/)

双击下载下来的 deb 安装文件进行安装。

注销当前用户并重新登录，在 Input Method 中将 Input method 选择为 Fcitx 输入法框架。

注销当前用户并重新登陆，在 Fcitx Configuration 中添加 Sogou Pinyin 输入法（添加时记得点掉 Only Show Current Language 复选框）。

注销当前用户并重新登陆，按 Ctrl + 空格键 切换中英文输入法（然后搜狗输入法就会常驻，只能按 Shift 键切换中英文）。
