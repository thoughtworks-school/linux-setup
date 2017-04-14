# 安装方法

## 安装镜像下载地址

- [Ubuntu 17.04](http://releases.ubuntu.com/17.04/ubuntu-17.04-desktop-amd64.iso)

## 语言选择

- 为了开发效率、学习质量和便于适应英文工作环境，请在安装时务必选择英文（美国）版本，举个例子来说，如果你是用的是中文版本，则在未来使用中是无法用 Dash 做到快速应用跳转，也很难在命令行快速进入中文文件目录的。

## 制作USB启动盘

- 准备一个容量大于 4GB 的U盘（请提前将U盘中内容备份，然后使用 FAT32 格式格式化该U盘）；
- 在 Windows 操作系统下使用 [Rufus USB Installer](https://rufus.akeo.ie/?locale=zh_CN/) 选择下载的安装镜像（ISO）文件并选择U盘所在盘符制作USB启动盘。

## 通用安装流程

**该部分是为了节省后续篇幅所描述的安装过程中通用的部分，并不完整，具体安装流程请以后续部分为准。**

**前序流程：**

0. 使用制作好的 USB 启动盘引导计算机，在 Ubuntu 引导界面选择 `Install Ubuntu` 开始安装程序。
0. 在 Welcome 界面选择系统语言为 English，然后点击 `Install Ubuntu` 开始安装。
0. 在 Preparing to install Ubuntu 界面，勾选 `Install third-party software for graphics and Wi-Fi hardware, Flash, MP3 and other media` 选项，以便未来安装一些有版权约束的软件或者无线网卡驱动。

**后续流程：**

0. 在 Where are you? 界面选择或输入时区为 `Shanghai`。
0. 在 Keyboard layout 界面，确保两个列表中选择的都是 `English (US)`。
0. 在 Who are you?  界面，依次填写你的全名、计算机名（可自动生成）、用户名、用户密码（会经常使用到）。
0. 完成安装并重启电脑。

## 干净安装

**该方法仅适合新电脑或者不准备继续使用Windows的情况。**

0. **请使用移动硬盘或者其它稳妥可靠的移动设备备份现有系统中的全部重要数据！**
0. （按照通用安装流程的前序部分操作）
0. 在 Installation type 界面 选择 `Erase disk and install Ubuntu` 选项擦除并使用全部硬盘进行安装。
0. （按照通用安装流程的后续部分操作）

## 双系统安装

首先，请检查当前电脑磁盘的分区方式是 MBR 分区方式还是 GPT 分区方式：[查看方法](http://jingyan.baidu.com/article/ad310e80a9298a1849f49e17.html)

然后，根据下列不同的分区方式，进行相应的安装流程。

#### MBR 硬盘分区表 + 以 Legacy BIOS 为引导方式的电脑

**常见于预装 Windows 7 的电脑**

0. **请使用移动硬盘或者其它稳妥可靠的移动设备备份现有系统中的全部重要数据！**
0. 在 Windows 操作系统下，使用磁盘分区工具（推荐使用 [EaseUS Partition Master Free](http://www.partition-tool.com/personal.htm)，安装时请仔细看清不要安装任何其捆绑的垃圾软件），在现有硬盘上调整出不少于 40GB 的干净硬盘空间（不要格式化），同时还要确保硬盘上除 Windows 系统分区这一个主分区以外，其他都是逻辑分区（可用工具转换主分区为逻辑分区）。
0. 将 BOIS 引导方式选为 `Legacy Only`。
0. （按照通用安装流程的前序部分操作）
0. 在 Installation type 界面 选择 `Install Ubuntu alongside Windows Boot Manager` 选项，安装程序将会利用划分出来的干净的硬盘空间自动分区并设置双系统引导程序。
0. （按照通用安装流程的后续部分操作）

#### GPT 硬盘分区表 + 以 UEFI 为引导方式的电脑

**常见于预装 Windows 8.1 / Windows 10 的电脑**

0. **请使用移动硬盘或者其它稳妥可靠的移动设备备份现有系统中的全部重要数据！**
0. 在 Windows 操作系统下，使用`磁盘管理`的`压缩卷`功能，从剩余空间最大的磁盘分区上压缩出不少于 60 GB 的干净硬盘空间（不要格式化）。
0. 将 BOIS 引导方式选为 `UEFI Only`。
0. 关闭 BIOS 中的 `CSM` 功能（有的话就关掉，没有的话就可以不用管）。
0. （按照通用安装流程的前序部分操作）
0. 在 Installation type 界面 选择 `Install Ubuntu alongside Windows Boot Manager` 选项，安装程序将会利用划分出来的干净的硬盘空间自动分区并设置双系统引导程序。
0. （按照通用安装流程的后续部分操作）
0. （可选）如果发现 Windows 关机后开机无法进入系统引导界面，可关闭 Windows 8.1 / Windows 10 中的快速启动功能：[查看关闭方法](http://jingyan.baidu.com/article/ca00d56c7a40e6e99febcf4f.html)