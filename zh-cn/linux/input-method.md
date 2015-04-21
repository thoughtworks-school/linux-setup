# 安装中文输入法

## Linux Mint

```bash
$ sudo apt-get update
$ sudo apt-get install ibus ibus-libpinyin
```

注销当前用户并重新登录，在 Keyboard Input Methods 中添加 Intelligent Pinyin 输入法，并且在输入法设置中关闭 Correct pinyin 功能。

## Ubuntu

```bash
$ sudo apt-get update
$ sudo apt-get install ibus-libpinyin
```

注销当前用户并重新登录，在 Text Entry 中添加 Intelligent Pinyin 输入法，并且在输入法设置中关闭 Correct pinyin 功能。

## Deepin

如果是中文版，则已预置搜狗拼音输入法。

如果是英文版，请在 Deepin Store 中安装 sogoupinyin ，然后重启，在 Fcitx Configuration 中添加 Sogou Pinyin，再重启后即可使用。
