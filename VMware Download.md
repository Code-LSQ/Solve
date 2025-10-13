https://github.com/201853910/VMwareWorkstation/releases
这是一个仓库，收集了官方的 VMware Workstation Pro 安装包。

https://packages.vmware.com/tools/releases/
VMware Tools 仓库

吾爱破解论坛的映梓制作了精简版，稳定性稍差一点，不过也很不错，我母亲正在用。
https://www.52pojie.cn/thread-1965033-1-1.html

VMware Workstation Pro 12.5.9 Build 7535481 PC&PE 精简注册版（-安装好即注册，原生虚拟磁盘映射功能，可根据需求个性化选择安装组件，支持Windows 7，硬件要求低）。
VMware Workstation Pro 15.5.7 Build 17171714 PC&PE.exe精简注册版（修改添加 DELL SLIC2.7 + MSDM + SLP + Virtual PC XP
-集成CDK，安装好即注册，原生虚拟磁盘映射功能，VM15最后一个支持Windows 7的版本，硬件要求中）。
VMware Workstation Pro 17.5.2 Build 23775571 PC&PE 精简注册版（修改添加 DELL SLIC2.7 + MSDM + SLP + Virtual PC XP
-集成CDK，安装好即注册，无虚拟磁盘映射功能，支持安装Windows 11虚拟系统，硬件要求高）,是最后一个未移除Unity模式、蓝牙等功能的版本。
等等。

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
