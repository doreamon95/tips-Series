---
title: "如何安装go环境(ubuntu16.04)"
tags: ["go"]
categories: ["go"]
date: "2019-06-20T21:00:00+08:00"
url: "/2019/6/20/go-env-install.html"
---

## 安装过程

首先可以在github查看自己想下载的github版本，官方链接为https://github.com/golang/go/releases，查看好之后用wget下载指定版本的go版本。比如下载1.12.6.

```
wget  https://dl.google.com/go/go1.12.6.linux-amd64.tar.gz
```

将下载之后的压缩包进行解压，得到解压版本

```
tar -xzf go1.12.6.linux-amd64.tar.gz 
```

## 配置环境

ubuntu16.04 root环境配置，打开 **/etc/profile** 以下信息：

```
export GOPATH=/opt/gopath
export GOROOT=/opt/go
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
```

配置好 /etc/profile 之后，source使配置环境变量生效

```
source /etc/profile
```

查看配置是否已经成功

```
go version
```

结果为：

```
go version go1.12.6 linux/amd64
```

