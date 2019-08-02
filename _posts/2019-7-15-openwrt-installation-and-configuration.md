---
layout: post
title: "What have I done"
tags: [openwrt,网络安全，开源]

以 Netgear R7800 为例
## 准备工作


### 硬件
`购买渠道：建议在亚马逊购买，其次是线下官方渠道`
#### u盘

#
#### Netgear R7800 路由器

#

### 软件
路由器固件下载至U盘
下载目录是：http://downloads.openwrt.org/
#
安装 tftp
linux（ubuntu）
`apt install tftp`
Mac OS
`brew install tftp`

System -- Administration 设置密码(关于[密码管理的建议](2019-7-20-suggestion-of-password-manage.md))

安装中文界面
```
opkg update
opkg install luci-i18n-base-zh-cn
```
如果使用 Windows to go 还会变成英文界面
(注意，有些路由器在图形界面，通过System -- Software 搜索 luci-i18n-base-zh-cn 是搜索不到的)

日志在 /var/log/messages 中查看
