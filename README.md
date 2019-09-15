# https://wzdh.github.io
我的永久GitHub网址导航

# https://github.com/wzdh/52share
我的永久软件分享站点

# 欢迎大家访问！！

# 一键安装wireguard 脚本 Debian 9 (源:逗比网安装笔记)
wget -qO- git.io/fptwc | bash

# 一键安装wireguard 脚本 Ubuntu   (源:逗比网安装笔记)
wget -qO- git.io/fpcnL | bash

# CentOS 7 一键脚本安装WireGuard  (官方脚本自动升级内核)
wget -qO- git.io/fhnhS | bash


CentOS 7 测试 GCP和Vultr 都能自动升级内核，如果辣鸡要升级内核
yum install -y wget vim             # Cetos 安装 wget 和 vim 工具
wget -qO wg.sh git.io/fhnhS && bash wg.sh kernel    # Centos 升级内核命令


[Peer]
PublicKey = QOb
Endpoint = 34.92.
AllowedIPs = 0.0.0.0/0, ::0/0
PersistentKeepalive = 25

#-----------------------------------------------------------------------
[Interface]
PrivateKey = YHWn
Address = 10.0.0.178/24, fd08:620c:4df0:65eb::178/64
DNS = 8.8.8.8, 2001:4860:4860::8888

[Peer]
PublicKey = QObNNx
Endpoint = 34.92.
AllowedIPs = 0.0.0.0/0, ::0/0
PersistentKeepalive = 25

#-----------------------------------------------------------------------
[Interface]
PrivateKey = qBt/2D5
Address = 10.0.0.186/24, fd08:620c:4df0:65eb::186/64
DNS = 8.8.8.8, 2001:4860:4860::8888

[Peer]
PublicKey = QObNNxFiJ+
Endpoint = 34.92
AllowedIPs = 0.0.0.0/0, ::0/0
PersistentKeepalive = 25

#-----------------------------------------------------------------------
   一键安装 WireGuard 脚本 For Debian_9 Ubuntu Centos_7   
     开源项目：https://github.com/hongwenjun/vps_setup    

# [信息] 新手使用 bash wg5  命令，使用临时网页下载配置和手机客户端二维码配置
# [信息] 推荐使用 bash wgmtu  命令，WireGuard 配置管理支持IPV6，稳定有待测试
# [信息] 自定端口 bash <(curl -L -s https://git.io/fpnQt)  9999 
# [信息] WG+SS域名分流升级命令  bash wgmtu setup 

# [信息] WireGuard是VPN协议，如果连上而没有回程流量，请使用 WG+SS 分流方案
# [信息] 客户端配置 AllowedIPs = 0.0.0.0/0, ::0/0 改成 AllowedIPs = 10.0.0.1/32 
# [信息] WG服务器相当于一个远程路由器，IP: 10.0.0.1,再开启一个SS，IP填  IP: 10.0.0.1 
[root@ssr-hongkong-c-20190913 ~]# 
