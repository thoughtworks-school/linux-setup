# 安装媒体播放器

## 媒体播放器的选择

我们推荐同时安装 [VLC media player](http://www.videolan.org) 和 [SMPlayer](http://smplayer.sourceforge.net) 两款媒体播放器，这样当遇到无法播放或者播放有问题的视频时能够有多一种选择。

## Linux Mint

### 安装 VLC media player

已预置，无需单独安装。

### 安装 SMPlayer

```bash
$ sudo add-apt-repository ppa:rvm/smplayer
$ sudo apt-get update
$ sudo apt-get install smplayer smtube smplayer-themes smplayer-skins
```

## Ubuntu

### 安装 VLC media player

```bash
$ sudo apt-get install vlc
```

### 安装 SMPlayer

```bash
$ sudo add-apt-repository ppa:rvm/smplayer
$ sudo apt-get update
$ sudo apt-get install smplayer smtube smplayer-themes smplayer-skins
```

## Deepin

内置的 Deepin 播放器非常强大，可以无需使用上述播放器。
