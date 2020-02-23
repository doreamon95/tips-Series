---
title: "如何安装阿里云ECS图形化界面(ubuntu16.04)"
tags: ["ecs"]
categories: ["ecs"]
date: "2019-11-19T21:00:00+08:00"
url: "/2019/11/19/ecs-ubuntu16.04-install.html"
---

步骤简要说明：

阿里云 ECS服务器版本： ubuntu16.04  抢占式  64bit

step1:  安装图形化界面操作

step2:  阿里云服务器后台进入图形化界面

​		    远程连接密钥是多少，要记住		比如：437493

step3:   阿里云控制台进行远程连接，下载teamviewer

​		 最好登录自己本地的teamviewer账号，并自己设置连接的密码

step4:   在自己电脑（win or linux)装上teamviewer进行远程ID连接

​		一般是输入密码即可匹配

step5:   关于屏幕分辨率匹配问题，teamviewer连接后一共才那几个选项，慢慢试，暂未找到好的解决方案。

下面**是亲测**可用的流程

------

## 安装图形化界面操作

更新软件源

**`# apt-get update`**

安装图形化界面（该步骤大概需要花2分钟）

**`# apt-get install ubuntu-desktop`**

重启

``` 
reboot
```

如需使用其他用户登录，需要修改**50-ubuntu.conf**配置文件

**`# vi /usr/share/lightdm/lightdm.conf.d/50-ubuntu.conf`**

修改为

```
[Seat:*]    
user-session=ubuntu    
greeter-show-manual-login=true     
allow-guest=false  
```

然后重启

`# reboot`

### 管理员控制台

进入**阿里云-控制台-ECS-选择自己的ECS服务器-远程控制**

此时会提示远程连接的验证码，只提示一次，务必记住

为确保万一，请设置自己的ECS的登录密码。

`username:root   password:请自行设置且记住`

此时已经登录进图形化界面了，接下来就是下载teamviewer

> 打开火狐浏览器，搜索 teamviewer，选择download，下载指定版本
>
> ♥ ubuntu16.04 64bit 下载 ubuntu支持的版本 .deb  x86 64位
>
> ♥ 下载完成，执行deb 进行 install即可
>
> ♥ 安装完毕，在software搜索teamviewer打开即可

打开teamviewer进行

> 🌹 首选登录自己teamviewer账号
>
> 🦋 在password旁边有个刷新按钮，点击选择 set personal password
>
> 这样会比较方便进行远程连接

### 本地teamviewer连接

最好可以在计算机和联系人这里添加远程计算机的连接方式