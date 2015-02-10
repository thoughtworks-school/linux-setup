# Linux 安装

## 安装镜像下载地址

- [Linux Mint 17.1](http://www.linuxmint.com/edition.php?id=172)
- [Ubuntu 14.10](http://www.ubuntu.com/download/desktop/thank-you?country=CN&version=14.10&architecture=amd64)

## 语言选择

- 为了学习质量和便于适应英文工作环境，请在安装时务必选择英文（美国）版本。

## 制作USB启动盘

- 准备一个容量大于4GB的U盘（请提前将U盘中内容备份，然后使用FAT32格式格式化该U盘）；
- 在Windows操作系统下使用 [Universal USB Installer](http://www.pendrivelinux.com/universal-usb-installer-easy-as-1-2-3/) 选择下载的安装镜像（ISO）文件并选择U盘所在盘符制作USB启动盘。

## 安装

**（安装时不要连接互联网，可以大幅度提高安装速度）**

### 干净安装

直接使用制作好的USB启动盘引导计算机，擦除并使用全部硬盘进行安装（该方法仅适合新电脑或者不准备继续使用Windows且做好备份的情况）。

### 双系统安装

0. 在Windows操作系统下，使用磁盘工具（推荐使用[EaseUS Partition Master Free](http://www.partition-tool.com/personal.htm)，安装时请仔细看清不要安装任何其捆绑的垃圾软件），在现有硬盘上划分出一个主分区（建议不要小于20GB，推荐60GB）和一个逻辑分区（与电脑内存大小一致）;
0. 使用 [EasyBCD](http://neosmart.net/EasyBCD/) 新建一个与安装的Linux发行版同名（比如 Linux Mint 或者 Ubuntu）的GRUB2引导项目，并将其位置指定在刚刚新划分出的主分区上；
0. 使用制作好的USB启动盘引导计算机，在安装向导中选择手动硬盘划分，选择新划分出的主分区，选择格式化为Ext4格式，并将```/```根目录指定到该分区上；
0. 选择新划分出的逻辑分区，并制定该分区为Swap分区；
0. 将引导分区盘符指定为新划分出的主分区（**这一步非常重要，切记！**）；
0. 按照安装向导完成后续安装步骤。
