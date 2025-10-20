
### VMware Workstation

这是关于 VMware Workstation 的一些资源和杂谈。

#### VMware Workstation Pro

我这里准备了 VMware Workstation Pro 的相关资源，内有精简版的12.5.9、15.5.7、17.5.2和原版的17.6.4 ，还有几个版本的 VMware Tools。

下载地址
https://www.123865.com/s/0Iv8Td-ARFMv?pwd=L123#


官方原版
https://github.com/201853910/VMwareWorkstation/releases
这是一个仓库，收集了官方的 VMware Workstation Pro 安装包。

VMware Workstation Pro 17 官方文档
https://techdocs.broadcom.com/cn/zh-cn/vmware-cis/desktop-hypervisors/workstation-pro/17-0.html

另外，很多人提到了 VMware Workstation Pro 的版本区别，但是没提到 VMware Tools 的版本区别，可以看本文下面 VMware Tools 那一段。


#### 精简版

精简注册版来自吾爱破解论坛的映梓。原帖地址：
https://www.52pojie.cn/thread-1965033-1-1.html

VMware Workstation Pro 12.5.9 Build 7535481 PC&PE 精简注册版（-安装好即注册，原生虚拟磁盘映射功能，可根据需求个性化选择安装组件，支持Windows 7，硬件要求低）。

VMware Workstation Pro 15.5.7 Build 17171714 PC&PE.exe精简注册版（修改添加 DELL SLIC2.7 + MSDM + SLP + Virtual PC XP
-集成CDK，安装好即注册，原生虚拟磁盘映射功能，VM15最后一个支持Windows 7的版本，硬件要求中）。

VMware Workstation Pro 17.5.2 Build 23775571 PC&PE 精简注册版（修改添加 DELL SLIC2.7 + MSDM + SLP + Virtual PC XP
-集成CDK，安装好即注册，无虚拟磁盘映射功能，支持安装Windows 11虚拟系统，硬件要求高）,是最后一个未移除Unity模式、蓝牙等功能的版本。


安装方法：
双击.exe可静默安装到默认目录，耐心等待程序自解压绿化完成，桌面就会出现VMware和vmplayer快捷方式图标，同时会自动启动VMware程序
或右键解压到任意目录，双击vmware目录下的setup.cmd安装

卸载方法：
双击vmware目录下的!)卸载.cmd卸载完成后，删除C:\Program Files\VMware文件夹即可


主要特色：
-修改添加 APPLE OSK，可以安装 MAC OS X（无需再使用Unlocker MacOS 解锁补丁：https://github.com/DrDonk/unlocker/releases/、https://github.com/DrDonk/unlocker/archive/master.zip）

-集成CDK，安装好即注册

-集成VC运行库，在未安装VC运行库的系统上也能正常运行

-BIOS 支持OEM激活 Windows XP, 2003, 2003R2, Vista, 2008, Win7, 2008R2, 2012, 2012R2, 2016, 2019、2022、2025

-EFI BIOS 支持OEM激活 Vista, 2008, Win, 2008R2, 2012, 2012R2, 2016, 2019、2022、2025

-VISTA~2025 对安装盘无要求，导入OEM证书和系统版本对应的OEM-CDK即可激活（DELL SLIC2.7证书、CDK自行搜索）

若修改并用 EFI BIOS，编辑虚拟机设置 – 选项 – 高级 – 勾选“通过 EFI 而非 BIOS 引导
比原版体积减小数倍，功能实用性强，可在PC和PE上运行，极为便捷。

#### 本人补充

对于精简版，如果有无法卸载的几个驱动程序，用 Geek Unistaller 选择强制删除，基本可以卸载干净。

精简版可以搭配映梓制作的 Windows 10 虚拟机使用
https://www.52pojie.cn/thread-1852714-1-1.html

或者我这里也要有一个基于该虚拟机的再修改版本，压缩前大概6GB，压缩后1.84GB。下载地址
https://www.123865.com/s/0Iv8Td-9RFMv?pwd=L123#
**免责声明：注意！未深入测试稳定性！！！生产环境请勿使用！！！如有意外，本人概不负责！！！**

另外，此虚拟机中不含有 WebView2 组件（原版和我的版本都是），基于该组件的应用无法运行，请自行安装该组件。

WebView2 下载
https://developer.microsoft.com/zh-cn/microsoft-edge/webview2/?form=MA13LH


#### VMware Tools

VMware Tools 仓库
https://packages.vmware.com/tools/releases/

VMware Tools 官方文档
https://techdocs.broadcom.com/cn/zh-cn/vmware-cis/vsphere/tools/12-0-0.html


VMware Tools 12.4.0 及更高版本已弃用 Unity 模式。

VMware Tools 12.5.3 及更高版本不再支持简体中文。使用已弃用语言的用户将不会再收到这些语言的更新或支持。


#### Unity

VMware Workstation Pro 17.5.2，说是最后一个未移除Unity模式、蓝牙等功能，但有人声称其内置的 VMware Tools 已经不再支持 Unity 模式，实测确实如此。解决方法为在应用中卸载 VMware Tools，给虚拟机安装较旧的 VMware Tools （手动拖放文件后双击运行安装，不要用内置的安装功能）。如 12.0.0、12.3.0。

Unity 模式是一种显示方式，允许虚拟机中的应用程序直接显示在主机系统的桌面上，就像一个单独的程序一样运行。你可以理解为把虚拟机里的窗口单独拖到外面。
我听说玩 Galgame 和装流氓软件（QQ、微信、WPS）用的多。


#### 空间清理

由于 VMware Workstation 的安装机制，它的 .exe 安装包在运行时会产生一个 .msi 安装包再安装，删除完全不影响使用。

C:\Program Files\Common Files\VMware\InstallerCache
虚拟机中安装 VMware Tools 时会在这里产生一个 .msi 文件（每个版本都会），几十M大小。

C:\Program Files (x86)\Common Files\VMware\InstallerCache
在物理机上安装官方的原版 VMware Workstation 时，会在这产生一个 .msi 文件（估计也是每个版本都会），几百M大小。

此外如果使用 VMware 内置的在线更新功能，它会在 AppData 下产生一个 .exe 文件，安装完不删除。

这是我在清理硬盘的时候发现的，很少有人提到我就说一下。


#### 其他

脚本一键启动虚拟机，注意改成自己的路径
"C:\Li\Tool\VMware Workstation\vmrun.exe" -T ws start "C:\Li\Virtual Machines\Kali Linux\Kali Linux.vmx" gui

安装完成后可以移除 CD/DVD 驱动器，不影响使用。

安装 Windows 时，最好先不要给虚拟机联网。

如果你没有多个CPU，虚拟机处理器数量，选择一个，处理器核心数量，不超过线程数，也就是任务管理器中 CPU 的逻辑处理器数量。

