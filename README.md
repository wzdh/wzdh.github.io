# https://wzdh.github.io
我的永久GitHub网址导航

# https://github.com/wzdh/52share
我的永久软件分享站点
==========================================================================================================================
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
==========================================================================================================================
★★★★★阿里云香港轻量服务器V2RAY一键安装教程
==========================================================================================================================
创建完香港轻量应用服务器（建议选择Debian 9+ 系统镜像，脚本会自动启用 BBR 优化）后，登录轻量应用服务器控制台：
第一步：重置root密码为Fuckgfw****
第二步：修改防火墙规则：添加规则，应用类型：全部TCP+UDP，点击确定完成。
第三步：远程连接：输入sudo su root切换至root账号。

第四步：运行233boy博客的一键安装V2Ray脚本，使用 root 用户输入下面命令安装或卸载V2Ray
bash <(curl -s -L https://git.io/v2ray.sh)
使用tcp传输协议，端口选择33889，其他全部选择N，一路Next，直至安装成功。
选用脚本：bash <(curl -s -L https://233v2.com/v2ray.sh)

第五步：卸载、屏蔽安骑士
1.首先卸载阿里云安骑士，教程转自：https://www.wn789.com/11468.html
wget http://update.aegis.aliyun.com/download/uninstall.sh && chmod +x uninstall.sh
./uninstall.sh 
wget http://update.aegis.aliyun.com/download/quartz_uninstall.sh && chmod +x quartz_uninstall.sh
./quartz_uninstall.sh
2.删除残留文件
pkill aliyun-service
rm -fr /etc/init.d/agentwatch /usr/sbin/aliyun-service
rm -rf /usr/local/aegis*
3.屏蔽安骑士 IP
iptables -I INPUT -s 140.205.201.0/28 -j DROP 
iptables -I INPUT -s 140.205.201.16/29 -j DROP 
iptables -I INPUT -s 140.205.201.32/28 -j DROP 
iptables -I INPUT -s 140.205.225.192/29 -j DROP 
iptables -I INPUT -s 140.205.225.200/30 -j DROP 
iptables -I INPUT -s 140.205.225.184/29 -j DROP 
iptables -I INPUT -s 140.205.225.183/32 -j DROP 
iptables -I INPUT -s 140.205.225.206/32 -j DROP 
iptables -I INPUT -s 140.205.225.205/32 -j DROP 
iptables -I INPUT -s 140.205.225.195/32 -j DROP 
iptables -I INPUT -s 140.205.225.204/32 -j DROP

第六步：安装BBR +：
注意：要先选择第2项：安装 BBRplus版内核，然后重启VPS后，再次运行./tcp.sh选择第7项：使用BBRplus版加速
1.sudo su root
2.yum install -y wget
3.wget --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh
4../tcp.sh #注：安装过程中，提示是否中止删除低版本的内核，选择"N"，意思是不中止，让脚本自动删除低版本的内核。
5.reboot   #重启VPS
6.sudo su root
7../tcp.sh

第七步：重启VPS，开启FQ愉快之旅。

==========================================================================================================================
★★★★★3条命令快速在谷歌云安装BBR PLUS加速和SSR
==========================================================================================================================
安装脚本支持系统Centos 6+ / Debian 7+ / Ubuntu 14+，BBR魔改版不支持Debian 8
机器类型: 选微型(一个共享vCPU)
0.6G内存, 一般加速上网, 看视频, 玩游戏都够用了. 后续也可以更改成小型或更高的.
启动磁盘: 默认是Debian, 推荐改成CentOS 7.
以下命令都是基于CentOS 7 64位, 如选Debian, Ubuntu等其他系统, 命令会稍有不同, 自行解决.

一、安装千影：BBR+BBR魔改版+BBRplus+Lotserver：
注意：要先安装BBR PLUS内核，然后重启VPS后，再次运行./tcp.sh安装BBR plus 加速程序
1.sudo -i
2.yum install -y wget
3.wget --no-check-certificate https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh && chmod +x tcp.sh
4../tcp.sh
5. reboot重启VPS
6.sudo -i
7../tcp.sh
二、安装shadowsocksR脚本：
1.sudo -i
2.wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh && chmod +x shadowsocksR.sh
3../shadowsocksR.sh
https://www.94ish.me/1635.html

GitHub源码地址：
https://github.com/teddysun/shadowsocks_install/tree/master
https://github.com/teddysun/across
秋水逸冰博客：https://teddysun.com/
Linux网络优化加速一键脚本：https://github.com/chiakge/Linux-NetSpeed

外贸SOHO笔记:Google Cloud Platform免费申请&一键搭建SSR & BBR加速教程
https://www.wmsoho.com/google-cloud-platform-ssr-bbr-tutorial/

秋水逸冰的BBR不好手：最好先运行BBR加速脚本，再安装shadowsocksR
1.sudo -i
2.yum install -y wget
3.wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh
4../bbr.sh
==========================================================================================================================
