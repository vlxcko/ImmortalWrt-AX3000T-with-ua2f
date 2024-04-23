# OpenWRT-CI
云编译OpenWRT固件
（小米AX3000T专用）

LEDE源码：
https://github.com/coolsnowwolf/lede （不再自动编译）

IMMORTALWRT源码：
https://github.com/immortalwrt/immortalwrt

# 固件简要说明：

固件每周五早上4点自动编译。(天天更新真没必要，本来想做个检测上游代码改动来决定是否编译的)

固件信息里的时间为编译开始的时间，方便核对上游源码提交时间。

默认附带的软件包可以在`Scripts`和`Config`内查看，也可安装后自行安装需要的软件包.

推荐安装后更换opkg源为校园网联合镜像站源，操作方法详见[https://help.mirrors.cernet.edu.cn/immortalwrt](https://github.com/VIKINGYFY/UBOOT-CI/releases).

# 固件安装简要说明：

含ubootmod的固件需要先刷入Release内同样的Uboot.

普通固件请刷入[https://github.com/VIKINGYFY/UBOOT-CI/releases](https://github.com/VIKINGYFY/UBOOT-CI/releases)内对应型号的Uboot.

Uboot地址为`192.168.1.1`，更多操作方法详见[https://cmi.hanwckf.top/p/mt798x-uboot-usage/](https://cmi.hanwckf.top/p/mt798x-uboot-usage/)

Uboot分区布局请选择默认.

# 目录简要说明：

Depends.txt——环境依赖列表

workflows——自定义CI配置

Scripts——自定义脚本

Config——自定义配置
