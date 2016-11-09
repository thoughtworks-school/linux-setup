# 设置软件源并更新系统

0. 在 Software & Updates 的 Other Software 选项卡中，勾选全部 Canonical Partners 源。
0. 利用下方的 Close 按钮关闭 Software & Updates，在弹出的提示框中点击 Reload 按钮更新软件源信息。
0. 使用 Software Updater 更新系统。
0. 在 Language Support 中，根据系统提示安装缺失的语言文件。

## 如果你发现更新速度过慢（仅当出现问题之后使用）

如果你在安装 Ubuntu 的时候选择了正确的时区，那么 Ubuntu 会默认使用名为 `Server for China` 的软件源服务器，这个服务器现在默认是架设在国内的阿里云服务上的，所以国内的下载速度理应不会太慢。

但是如果你发现更新或者安装软件包的时候的下载速度过慢，可以尝试修改软件源：

0. 在 Software & Updates 的 Ubuntu Software 选项卡中，点击 Download from 下拉框，在 Other 中，在中国地区的源服务器中选择经过测试下载最快速的服务器（请见下表），并使用 Choose Server 按钮选定（很重要，节省接下来大量的时间）。
0. 利用下方的 Close 按钮关闭 Software & Updates，在弹出的提示框中点击 Reload 按钮更新软件源信息。
0. 使用 Software Updater 更新系统。

### 经测试下载最快速的软件源服务器列表

此列表需要持续补充。

| 所在学校名称 | 源服务器地区分类   | 源服务器地址        | 连接协议   | 服务器所有者     |
| :--------:   | :----------------: | :------------:      | :--------: | :-----------:    |
| 西安邮电大学 | China              | mirrors.aliyun.com/ubuntu | HTTP       | 阿里云 |
