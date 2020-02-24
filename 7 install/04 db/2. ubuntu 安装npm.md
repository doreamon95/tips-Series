---
title: "安装node和npm(ubuntu18.04/16.04)"
tags: ["npm"]
categories: ["Tool"]
date: "2020-02-24T21:00:00+08:00"
url: "/2020/02/24/node-npm-install.html"
---

1. 先更新一下源

```
sudo apt-get update
```

2. 先安装node

```
sudo apt-get install nodejs
sudo apt install nodejs-legacy
sudo apt install npm
```

3. 可更换淘宝镜像

```
sudo npm config set registry https://registry.npm.taobao.org
sudo npm conifg list #查看设置是否生效
```

4. 然后安装npm更新版本工具

```
sudo npm install n -g
sudo n stable #更新node版本
```

安装npm，https://github.com/npm/npm/releases

![](https://doreamon95.oss-cn-chengdu.aliyuncs.com/img/003/blog20200223145941.png)

