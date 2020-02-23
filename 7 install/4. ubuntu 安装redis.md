---
title: "安装redis与启动redis(ubuntu18.04)"
tags: ["redis"]
categories: ["redis"]
date: "2019-09-19T21:00:00+08:00"
url: "/2019/09/19/redis-ubuntu18.04-install.html"
---

## 前提说明

用途：Redis是常用基于内存的Key-Value数据库，这里用作缓存。

## 准备工作

### 安装

```
# 如果直接apt下载需要先更新apt
sudo apt update
# 从apt安装
sudo apt-get install redis-server
```

### 设置密码

```
# 打开
sudo vim /etc/redis/redis.conf
# 定位到 # requirepass foobared 去掉注释
requirepass 123456
```

## 开启远程访问

默认情况下，Redis服务器不允许远程访问，只允许本机访问，所以我们需要设置打开远程访问的功能。

```
# 打开Redis服务器的配置文件redis.conf
sudo vim /etc/redis/redis.conf
# 注释掉 bind 127.0.0.1这行  
bind 127.0.0.1  #把这个注释掉
```

### Redis命令

启动

```
sudo systemctl start redis
```

关闭

```
sudo systemctl stop redis
```

重启

```
sudo systemctl restart redis
```

## 连接测试

直接输入`redis-cli`通过默认客户端来测试连接，正常情况下返回`ping`的对应值PONG

![](https://doreamon95.oss-cn-chengdu.aliyuncs.com/img/001/sgx20200221103004.png)