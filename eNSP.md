
eNSP 需要 VirtualBox、WinPcap、Wireshark 作为运行环境。Wireshark的旧版本安装时可选安装WinPcap，但新版本已不再有此选项，需独立安装，或者你去安装旧版本，似乎要 3.0 以前的版本。

安装顺序建议为 WinPcap、Wireshark、VirtualBox、eNSP。

eNSP V100R003C00SPC100，这个版本是 eNSP 最后的正式版。建议安装VirtualBox 5.2.44，有的版本存在兼容性问题。如果是 eNSP V100R002C00B510，应该也可以用VirtualBox 5.2.44，不过我没试。Wireshark的兼容性我不清楚，最新的4.6.0应该兼容，另外Wireshark有安装 Npcap 的选项，不清楚选择安装是否会导致兼容性问题。

如果安装时出了问题可以用 Geek Uninstaller 卸载后再安装。

VirtualBox历史版本下载： https://download.virtualbox.org/virtualbox/

Wireshark下载： https://www.wireshark.org/download.html

eNSP V100R003C00SPC100、VirtualBox 5.2.44、Wireshark 4.6.0、WinPcap 4.1.3，打包下载地址  https://www.123865.com/s/0Iv8Td-yOFMv?pwd=L123#

如果 Wireshark 中文显示异常，去看本仓库的解决 Qt 中文显示异常。

