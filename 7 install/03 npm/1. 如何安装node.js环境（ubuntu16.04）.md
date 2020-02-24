---
11title: "如何安装node.js环境(ubuntu16.04)"
tags: ["nodejs"]
categories: ["nodejs"]
date: "2019-11-19T21:00:00+08:00"
url: "/2019/11/19/node-env-install.html"
---

## 下载安装

首先下载10.x版本的node，比如安装10.x

```csharp
wget -qO- https://deb.nodesource.com/setup_10.x | sudo -E bash -
sudo apt-get install -y nodejs
```

安装npm

```
sudo apt install npm
```

升级

```
npm i -g npm  //最新版本
npm i -g npm@6.11.3//指定版本
```

查看Node和npm的版本

```
xuperxuperunion:EOS_wallet# node -v
v10.17.0
xuperxuperunion:EOS_wallet# npm -v
6.11.3
```

## 初始化操作

输入npm来进行初始化

```
npm init
```

npm initnpm install

初始化完毕需要安装.json配置里面的依赖

```
npm install
```
