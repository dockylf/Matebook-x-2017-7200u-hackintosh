# Matebook-x-2017-7200u-hackintosh

概况Profile

机型Model：Huawei Matebook X 2017

处理器Processor：Intel i5-7200u

显卡Graphics: Intel HD Graphics 620

系统System：Ventura 13.0.1/Windows 10

引导/Boot：Opencore 0.8.6

可用Available: 无线网络、蓝牙、显卡、触控板、热键、背光、声卡、电池Wifi\bluetooth\Graphics\Trackpad\Hotkey\Brightness\Audio\Battery

不可用Unavailable: 指纹、隔空投送Fingerprint\Airdrop

Hidpi:网上教程很多，可以参考dortania.io的post-install部分，codeclou.io的方法，用hackintool和自带的终端实现，或者用one-key-hidpi脚本，这里不过多描述。please check dortania.io and codeclou.io, and use hackintool and terminal, or you can use one-key-hidpi, I won't talk about the details here.

蒙特雷For Monterey:如想在蒙特雷上使用，请先替换网卡驱动为2.1.0稳定版，不然会反复重启。replace airportitlwm_ventura with airportitlwm 2.1.0 stable before you use this efi.

Trim:为提升开机速度，我已关闭启动期间的trim保护(原开机时间1分35秒，关闭后开机时间25秒），请使用sensei工具重新确认系统运行期间Trim已关闭，或在config.plist中重新打开启动期间的trim保护（SetApfsTrim Timeout设置为-1即开启保护，设置为0即关闭保护）。To speed up booting(time reduce from 1'35“ to 25")，I've set SetApfsTrimTimeout to 0, please confirm the Trim is on with Sensei.app to protect your ssd, or you can set SetApfsTrimTimeout back to -1.

# Credit 致谢

大头蔡Cass for trim

澎湖冰洲，神楽小白 for Trackpad fix

LEONLIIIIII for fix EFI.
