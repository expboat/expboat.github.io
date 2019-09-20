---
layout: post
entitle: "openwrt-installation-and-configuration"
title: "配置安全的路由器"
categories: [路由器,openwrt,网络安全]
permalink: '/openwrt-installation-and-configuration'
---

简版教程请阅读 -->

反馈邮箱： bettersicsurf[at]outlook[dot]com, 反馈*博客出现的错误，需要改进的地方* , 此邮箱*不回复*读者，提前感谢你的反馈:)
个人邮箱： (**PS: remember remove the space below**): `dXNpbmdfX2VtYWlsOjxleHBib2F0W2F0XXBtLm1lPl9fd2l0aF9wZ3BfdW50aWxsXzIwMjAwNjAx Cg==`
推荐阅读：[如何注册，使用 tutanota.com](#)



## 注意事项

-   18.06 及后来的版本`不支持`储存小于 4MB FLASH / 32MB RAM 的设备

部分路由器 选择 Netgear Linksys Asus


ASUS RT-AC68U  ￥700


糟糕的路由器，利用漏洞，通过转发包到指定服务器

- 查看 更新频率
  官网

- 查看 漏洞暴露频率


选择支持openwrt路由器，搜索到`对应型号的教程` (最好教程下方有「安装成功」这类评论)， 然后购买
    相关文章--\[]如何使用搜索引擎](/how-to-use-search-engine)

<br>
以 Netgear R7800 为例
## 准备工作

### 硬件

购买渠道：`建议在线下官方渠道购买，其次是亚马逊购`

#### u盘

u盘
<br>

#### Netgear R7800 路由器

<br>

### 软件

路由器固件下载至U盘
下载目录是：<http://downloads.openwrt.org/>

#

安装 tftp
linux（ubuntu）
`apt install tftp`
Mac OS
`brew install tftp`

System -- Administration 设置密码(关于[密码管理的建议](2019-7-20-suggestion-of-password-manage.md))

安装中文界面

    opkg update
    opkg install luci-i18n-base-zh-cn

如果使用 Windows to go 还会变成英文界面
(注意，有些路由器在图形界面，通过System -- Software 搜索 luci-i18n-base-zh-cn 是搜索不到的)

日志在 /var/log/messages 中查看
