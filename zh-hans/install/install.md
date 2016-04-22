# 安装方法

## 安装镜像下载地址

- [Ubuntu 16.04 LTS](http://releases.ubuntu.com/16.04/ubuntu-16.04-desktop-amd64.iso)

## 语言选择

- 为了开发效率、学习质量和便于适应英文工作环境，请在安装时务必选择英文（美国）版本。

## 制作USB启动盘

- 准备一个容量大于4GB的U盘（请提前将U盘中内容备份，然后使用FAT32格式格式化该U盘）；
- 在Windows操作系统下使用 [Universal USB Installer](http://www.pendrivelinux.com/universal-usb-installer-easy-as-1-2-3/) 选择下载的安装镜像（ISO）文件并选择U盘所在盘符制作USB启动盘。

## 安装

**（如所在网络的国外访问速度较低，安装时请不要连接互联网，这样可以大幅度提高安装速度）**

### 干净安装

0. **请使用移动硬盘或者其它稳妥可靠的移动设备备份现有系统中的全部重要数据！**
0. 直接使用制作好的USB启动盘引导计算机，擦除并使用全部硬盘进行安装（该方法仅适合新电脑或者不准备继续使用Windows的情况）。

### 双系统安装

#### MBR 硬盘分区表 + 以 Legacy BIOS 为引导方式的电脑

0. **请使用移动硬盘或者其它稳妥可靠的移动设备备份现有系统中的全部重要数据！**
0. 将 BOIS 引导方式选为 Legacy Only。
0. 在Windows操作系统下，使用磁盘工具（推荐使用[EaseUS Partition Master Free](http://www.partition-tool.com/personal.htm)，安装时请仔细看清不要安装任何其捆绑的垃圾软件），在现有硬盘上划分出一个主分区（建议不要小于20GB，推荐60GB）和一个逻辑分区（2GB）;
0. **以 Linux 为双系统引导入口的安装方法（推荐）：**
  0. 使用制作好的USB启动盘引导计算机，在安装向导的安装方式选择截面中，选择 Something else 手动划分硬盘分区，选择新划分出的主分区，选择格式化为Ext4格式，并将```/```根目录指定到该分区上；
  0. 选择新划分出的逻辑分区，并指定该分区为Swap分区；
  0. 按照安装向导完成后续安装步骤。
0. **以 Windows 为双系统引导入口的安装方法：**
  0. 使用 [EasyBCD](http://neosmart.net/EasyBCD/) 新建一个与安装的Linux发行版同名（比如 Linux Mint 或者 Ubuntu）的GRUB2引导项目，并将其位置指定在刚刚新划分出的主分区上；
  0. 使用制作好的USB启动盘引导计算机，在安装向导的安装方式选择截面中，选择 Something else 手动划分硬盘分区，选择新划分出的主分区，选择格式化为Ext4格式，并将```/```根目录指定到该分区上；
  0. 选择新划分出的逻辑分区，并指定该分区为Swap分区；
  0. 将引导分区盘符指定为新划分出的主分区（**这一步非常重要，切记！**）；
  0. 按照安装向导完成后续安装步骤。

#### GPT 硬盘分区表 + 以 UEFI 为引导方式的电脑

**常见于预装 Windows 8.1 / Windows 10 的电脑**

0. **请使用移动硬盘或者其它稳妥可靠的移动设备备份现有系统中的全部重要数据！**
0. 关闭 Windows 8.1 / Windows 10 中的快速启动功能：[查看关闭方法](http://jingyan.baidu.com/article/ca00d56c7a40e6e99febcf4f.html)
0. 关闭 BIOS 中的 Secure Boot 功能
0. 关闭 BIOS 中的 QuickBoot/FastBoot，Intel Smart Response Technology (SRT)，Fast Startup，CSM支持功能（有的话就关掉，没有的话就可以不用管）。
0. 将 BOIS 引导方式选为 UEFI Only，其他硬件或者输入设备启动方式使用 Legacy 方式或者保持不变。
0. 在Windows操作系统下，使用磁盘工具（推荐使用[EaseUS Partition Master Free](http://www.partition-tool.com/personal.htm)，安装时请仔细看清不要安装任何其捆绑的垃圾软件），在现有硬盘上划分出一个较大的分区（建议不要小于20GB，推荐60GB）和一个较小的分区（2GB）;
0. **以 Linux 为双系统引导入口的安装方法（目前唯一问题最少的方式）：**
  0. 使用制作好的USB启动盘引导计算机，在安装向导的安装方式选择截面中，选择 Something else 手动划分硬盘分区，选择新划分出的较大的分区，选择格式化为Ext4格式，并将```/```根目录指定到该分区上；
  0. 选择新划分出的较小的分区，并指定该分区为Swap分区；
  0. 按照安装向导完成后续安装步骤。
