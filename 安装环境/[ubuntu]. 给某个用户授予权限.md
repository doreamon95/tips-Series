---
title: "ubuntu给某个用户授予操作某个文件夹权限"
tags: ["linux"]
categories: ["Tool"]
date: "2020-2-23T21:00:00+08:00"
url: "/2020/2/23/ubuntu-chown-1.html"
---

1. root账户登录

   ```
   sudo su  # or su root
   ```

2. 给用户授予权限，比如

   ```
   chown -R user file
   # chown -R doreamon /opt
   ```

   

