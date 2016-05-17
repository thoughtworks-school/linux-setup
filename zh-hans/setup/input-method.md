# 安装中文输入法

经过测试，系统自带的基于 IBus 输入法框架的 Intelligent Pinyin 是目前兼容性最好且最为稳定的中文输入法，只是词库不够智能。

而搜狗输入法 Linux 版因为存在的兼容性问题和键位冲突问题太多，所以不推荐使用。

## IBus 输入法框架 + Intelligent Pinyin 输入法

```bash
sudo apt update
sudo apt install ibus-libpinyin
```

确认在 Language Support 中将 Keyboard input method system 选择为 IBus 输入法框架。

注销当前用户并重新登录，在 Text Entry 中添加 Intelligent Pinyin 输入法。

在 Text Entry 界面的输入法列表中选中 Intelligent Pinyin 项，然后点击列表下方的工具按钮打开输入法设置界面，在 Pinyin mode 选项卡中取消勾选 Enable correct pinyin，这个选项会令输入法行为变得非常古怪。

成功后按 Windows徽标键 + 空格键 切换中英文输入法。
