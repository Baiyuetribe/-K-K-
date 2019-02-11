# 忆流年（艾K）发卡系统搭建教程

> 本教程最后于2019/2/10更新

## 前言

这是一款类material的主题，简化的UI让该系统特色鲜明。该发卡系统已适配自家的艾K支付，算是比较新的一款发卡系统，这种集成自家支付系统的发卡系统，已经成为主流。

演示地址：http://www.aikpay.cn/index.php  （此处仅为支付官网，发卡系统没有demo）

## 截图

![](https://ww1.sinaimg.cn/large/007i4MEmgy1g01pmlg9ezj30nb0ih0ud.jpg)

![](https://ww1.sinaimg.cn/large/007i4MEmgy1g01pnp8timj30nb0ifwfh.jpg)

![](https://ww1.sinaimg.cn/large/007i4MEmgy1g01pr7bqk0j30n70i70v2.jpg)

## 优点

- 简明的material主题
- 购买流程体验极佳
- 配合aikpay可以实现支付宝、微信、QQ收款
- 缺点：仅仅支持自家的aikpay，所以其它支付接口不可用

## 完整视频教程

![](https://ws1.sinaimg.cn/large/0072Lfvtly1fzoj7dw3l2j30dz01z3yb.jpg)

## 图文安装

**github地址**：https://github.com/Baiyuetribe/Ai.-K_faka

**环境要求： ** Mysql至`5.6+`、 `Nginx`、PHP 推荐`7.1`。（可安装至虚拟机）

### 1.安装宝塔

参考[宝塔教程](https://baiyue.one/%E7%BB%8F%E9%AA%8C%E8%AE%B0%E5%BD%95/275.html)

### 2.添加网站

LNMP环境部署完成后，打开宝塔面板，添加网站。

![](https://ws1.sinaimg.cn/large/0072Lfvtly1fzrq9b4lznj30hl0ct0t8.jpg)

### 3.源码安装

下载[源码](https://raw.githubusercontent.com/Baiyuetribe/Ai.-K_faka/master/%E8%89%BEK%E5%8F%91%E5%8D%A1%E7%B3%BB%E7%BB%9F%EF%BC%88%E8%89%BEK%E6%94%AF%E4%BB%98%E7%89%88%EF%BC%89.zip) ,然后本地上传至网站目录后解压。新建数据库，修改conn.php内的数据库

```
'database_name' => 'aikpay.cn',//数据库名 
'username' => 'aikpay.cn',//数据库用户名 
'password' => 'aikpay.cn',//数据库密码
```

![](https://ww1.sinaimg.cn/large/007i4MEmgy1g01pwjbutij30az0dhwf1.jpg)

### 4.数据库导入

把`www.aikpay.cn.sql`导入数据库。完成后即可访问，后台地址/admin 账号admin密码123456

## 其它备注

本站暂未测试其支付接口，有兴趣的可以按照后台提供的支付链接，注册aikpay的账号后尝试下。

博客来源： https://baiyue.one

**如果你想代搭建或定制，右转[佰阅小店](https://mall.baiyue.one)**
