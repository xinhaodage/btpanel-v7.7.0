# btpanel-v7.7.0
btpanel-v7.7.0-backup  官方原版v7.7.0版本面板备份

**Centos/Ubuntu/Debian安装命令 独立运行环境（py3.7）：**

```Bash
curl -sSO https://raw.githubusercontent.com/zhucaidan/btpanel-v7.7.0/main/install/install_panel.sh && bash install_panel.sh
```

跳过登录框，以及破解插件等请自行搜索

&nbsp;

**如果遇到重启后宝塔乱码 请DD最新版Debian系统然后修改语言区域：**


```Bash
nano /etc/default/locale
```

```Bash
LANG=en_US.UTF-8
```

修改后保存文件，重启VPS即可。


1、屏蔽强制绑定手机
```Bash
sed -i "s|bind_user == 'True'|bind_user == 'XXXX'|" /www/server/panel/BTPanel/static/js/index.js
```
2、直接删除宝塔强制绑定手机js文件
```Bash
rm -f /www/server/panel/data/bind.pl
```
##宝塔面板登录地址及账号密码查看命令##
```Bash
bt default
```
##bbrplus加速##
```Bash
wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
```
##查看开启状态##
```Bash
sysctl -p
```
##重启你的VPS##
```Bash
reboot
```
##登录宝塔面板安装套件##

##登录宝塔面板安装套件##
安装：Nginx1.18｜MySQL5.6｜php7.4
