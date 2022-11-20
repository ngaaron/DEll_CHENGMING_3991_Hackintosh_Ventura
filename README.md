# DEll_CHENGMING_3991_Hackintosh_Ventura
黑苹果 EFI文件，戴尔成铭3991主机核显输出，支持Ventura系统。

### EFI详情
* 支持MacOS版本：目前支持最新的Ventura 13.0版
* OpenCore版本：0.8.6
* 更新日期：2022年11月20日


### 配置清单
* 主板：DEll_CHENGMING_3991主机定制主板
* CPU：Intel i7-10700 八核心十六线程
* 显卡：核显 Intel UHD Graphics 630
* 网卡：BCM94360CS/BCM94360CD/BCM943602CS 都用过可以完美免驱
* 内存：海力士 DDR4 2933MHZ 8GX2 
* 固态硬盘：海康威视C2000 512G 
* 机械硬盘：西部数据 1T

### 完美程度
* 有线/无线耳机麦克风使用正常。
* 接力、随航功能正常使用。
* iMessage、FaceTime正常登陆使用。
* 有线网络/无线网络2G+5G正常使用。
* 前后各IO接口正常使用。
* 支持2k输出/4K未测试。
* 随眠唤醒不是100%成功。
* 其他问题欢迎反馈，目前还在继续完善中。

### BIOS推荐设置
* 关闭 Intel SGX
* 关闭 VT for Direct I/O
* 关闭 PTT（TPM设备）
* 关闭 CSM启动
* 关闭 Secure Boot 安全启动
* 开启 USB鼠标/键盘唤醒
* 开启 XHCI Hand-off（默认开启）
* 硬盘模式 SATA Mode: AHCI
* 其他设置似乎没有太大影响，我保持主板默认了。

### 使用说明
* 目前个人使用中支持BigSur和Monterey系统的安装和升级，并升级Ventura成功。

### 可能问题及解决方案
* 更新完系统后没有Hipi的话，可以使用one-key-hidpi-master脚本一键开启。
* 系统可以正常休眠，不过睡眠唤醒不是100%能成功，建议在节能中设置「防止系统进入睡眠」。
* 如果无法登陆使用iMessage和FaceTime等功能，可以自行替换三码和ROM参数，详细可以参考下方链接。

### Fixing iMessage and other services with OpenCore
* [https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#clean-out-old-attempts](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#clean-out-old-attempts)
