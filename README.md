# Linux-NetSpeed

说明：对于CentOS系统的BBR魔改之前搬运过南琴浪大佬的脚本，无奈出现了BUG，导致CentOS安装还存在着问题，前几天友链博主千影，也写出了一个魔改BBR脚本，脚本包含BBR+BBR魔改版+Lotsever(锐速)，同时支持Centos、Debian、Ubuntu系统，很方便，也很强大。

更新
新增南琴浪的暴力魔改BBR，使速度更加暴力，实际效果因线路而定。
安装
支持系统：Centos 6+/Debian 8+/Ubuntu 14+。
注意：该脚本在Vultr各个系统均测试通过，如果期间有出现任何问题，可向原作者反映帮助改善。
运行以下命令：

wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
Ubuntu 18.04魔改BBR暂时有点问题，可使用以下命令安装：

wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh"
apt install make gcc -y
sed -i 's#/usr/bin/gcc-4.9#/usr/bin/gcc#g' '/root/tcp.sh'
chmod +x tcp.sh && ./tcp.sh
如果还有更多系统安装有误的，可以及时反馈。

使用说明
使用脚本后会出现如下选项：
请输入图片描述
根据自己需求操作，重启后再使用./tcp.sh命令接着操作。

如果在删除内核环节出现这样一张图
请输入图片描述
注意选择NO，然后根据提示重启系统。

get -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
脚本内容如下


TCP加速 一键安装管理脚本 [v1.1.9]
 
0. 升级脚本
————————————内核管理————————————
1. 安装 BBR/BBR魔改版内核
2. 安装 Lotserver(锐速)内核
————————————加速管理————————————
3. 使用BBR加速
4. 使用BBR魔改版加速
5. 使用暴力BBR魔改版加速(不支持部分系统)
6. 使用Lotserver(锐速)加速
————————————杂项管理————————————
7. 卸载全部加速
8. 系统配置优化
9. 退出脚本
————————————————————————————————
 
当前状态: 已安装 Lotserver 加速内核 , 未安装加速模块
 
请输入数字 [0–9]:
如果删除内核过程中出现下图，选择no
