## 刷机推荐使用刷机工具进行操作

| 项目 | 信息 |
|------|------|
| 管理地址 | 192.168.10.1 root 无密码 |
| | |
| tailscale | tailscale在源安装 面板在https://github.com/Tokisaki-Galaxy/luci-app-tailscale-community/releases |
| smartdns | 若无ui或无法启动，可在软件包卸载后进ssh安装 /etc/smartdns-ipk 下的版本 |
| Mihomo | 下载安装https://github.com/nikkinikki-org/OpenWrt-nikki/releases |
| softethervpn-控制台 | 下载安装https://github.com/SoftEtherVPN/SoftEtherVPN |
| softethervpn-luci | 下载安装https://github.com/superzjg/luci-app-softethervpn |
| softethervpn | 下载安装https://github.com/SoftEtherVPN/SoftEtherVPN_Stable |

## 按需下载对应的工具和刷机包 执行刷机脚本即可（先安装9008驱动 然后 设备直接插电脑显示ADB设备后等10秒左右即可）
 - *-squashfs-system.img改名为system.img
 - *-squashfs-boot.img改名为boot.img

## 系统更新包
 - *-squashfs-sysupgrade.bin


## Credits(旧刷机方法)
- msm8916的包刷机 
- web在线升级没变化使用flash.zip线刷一下最新固件即可
-
- 想快速进bootloader模式线刷小技巧 重启就是bootloader模式了
- 系统内执行 dd if=/dev/zero of=/dev/mmcblk0p12 bs=4M sync
-
- 首次刷机下载仓库 flash.zip解压 注意不执行这一步无法开机
- immortalwrt-msm89xx-msm8916-openstick-jz02v10-squashfs-system.img改名为rootfs.img
- immortalwrt-msm89xx-msm8916-openstick-jz02v10-squashfs-boot.img改名为boot.img
- boot.img和rootfs.img放解压好的flash目录去！
- windows执行flash.bat刷机 linux系统执行./flash.sh刷机  
- 后续直接支持系统内在线升级刷机直接下载 immortalwrt-msm89xx-msm8916-openstick-jz02v10-squashfs-sysupgrade.bin 
- 其他机型按型号下载替换
- fsg.bin fsc.bin modemst2.bin modemst1.bin最好用自己机型的！！！


- [GitHub Actions](https://github.com/features/actions)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [immortalwrt](https://github.com/immortalwrt/immortalwrt)
- [lede](https://github.com/coolsnowwolf/lede)
