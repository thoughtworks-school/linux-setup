# 安装 Skype

Skype 是目前唯一能够跨平台，在 Linux 下支持文字、语音、视频沟通且世界流行的即时通讯工具，请使用微软帐号登陆。

```bash
curl https://repo.skype.com/data/SKYPE-GPG-KEY | sudo apt-key add -
```

```bash
echo "deb [arch=amd64] https://repo.skype.com/deb stable main" | sudo tee /etc/apt/sources.list.d/skype-stable.list
```

```bash
sudo apt update
sudo apt install skypeforlinux
```
