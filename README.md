# LuCI Rosy Theme

## About
Rosy is a concise and flat theme based on OpenWrt's web management interface. And it is based on luci-theme-material and JQ. **openwrt-18.06** branch is recommended if you are interested in this project.

## Usage
* If there's a previous LuCI in your buildroot, clone this project to one of directory under package/xxx.

* Otherwise you can use LuCI feed from [here](https://github.com/rosywrt/luci).

## Contact
* Bug Report : https://github.com/rosywrt/luci-theme-rosy/issues

**NOTE!!!** Currently, we don't maintain the issues led by images built from other source except [openwrt](https://github.com/openwrt/openwrt) and [luci](https://github.com/openwrt/luci).
Please report bugs to the corresponding owner.

* QQ Gourp : 428742246

## License
LuCI Theme Rosy: Copyright 2018 RosyWrt

LuCI Theme Material: Copyright 2015 Lutty Yang

LuCI Theme Bootstrap: Copyright 2012 Nut & Bolt

Licensed under the Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0

## Previews
### PC Login
<div align=center><img src="https://raw.githubusercontent.com/rosywrt/luci-theme-rosy/openwrt-18.06/previews/login-pc.png" alt="login-pc"/></div>

### PC Overview

<div align=center><img src="https://raw.githubusercontent.com/rosywrt/luci-theme-rosy/openwrt-18.06/previews/overview-pc.png" alt="overview-pc"/></div>

### iPad Login
<div align=center><img src="https://raw.githubusercontent.com/rosywrt/luci-theme-rosy/openwrt-18.06/previews/login-ipad.png" alt="login-ipad"/></div>

### iPad Overview

<div align=center><img src="https://raw.githubusercontent.com/rosywrt/luci-theme-rosy/openwrt-18.06/previews/overview-ipad.png" alt="overview-ipad"/></div>

### Mobile Login

<div align=center><img src="https://raw.githubusercontent.com/rosywrt/luci-theme-rosy/openwrt-18.06/previews/login-mobile.png" alt="login-mobile"/></div>

### Mobile Overview

<div align=center><img src="https://raw.githubusercontent.com/rosywrt/luci-theme-rosy/openwrt-18.06/previews/overview-mobile.png" alt="overview-mobile"/></div>


一、使用WinSCP登录路由器
1.文件协议选择 SCP
2.主机名,路由器的IP地址(通常为192.168.1.1 或 192.168.0.1 或 10.0.0.1 等等),端口默认 22
3.用户名(OpenWrt默认root),密码(通常为登录路由器web页面使用的密码,或者ssh的登录密码)
4.点击"保存(S)",然后点击"登录".

二、添加静态资源(CSS样式表,JS脚本文件,图片资源)
1.找到路径 /www/luci-static
2.复制主题资源文件夹 ../luci-static/FileName(通常为主题名) 到以上路径

三、添加页面模板(Luci的页面模板是由header.htm和footer.htm组成)
1.找到路径 /usr/lib/lua/luci/view/themes
2.复制主题资源 ../themes/FileName(通常为主题名) 到以上路径

四、编辑Luci配置文件
1.找到文件 /etc/config/luci
2.打开文件,并找到文件内容行 config 'internal' 'themes'
3.按照已有格式添加新的主题配置行,通常为 option '主题名称' '/luci-static/FileName(主题文件夹名称)'
4.保存并关闭文件,刷新路由器Web页面就可以找到新添加的主题了.
