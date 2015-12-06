# 安装中文输入法

经过测试，系统自带的基于 IBus 输入法框架的 Intelligent Pinyin 是目前兼容性最好且最为稳定的中文输入法，所以我们暂时不推荐使用搜狗输入法的 Linux 版本。

## Ubuntu

```bash
$ sudo apt-get update
$ sudo apt-get install ibus-libpinyin
```

注销当前用户并重新登录，在 Text Entry 中添加 Intelligent Pinyin 输入法，并且在输入法设置中关闭 Correct pinyin 功能。

## Linux Mint

```bash
$ sudo apt-get update
$ sudo apt-get install ibus ibus-libpinyin
```

注销当前用户并重新登录，在 Keyboard Input Methods 中添加 Intelligent Pinyin 输入法，并且在输入法设置中关闭 Correct pinyin 功能。
