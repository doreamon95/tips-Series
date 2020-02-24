---
title: "github私有仓库建立"
tags: ["github"]
categories: ["github"]
date: "2019-05-30T21:00:00+08:00"
url: "/2019/5/30/new-github-private.html"
---

## 新建仓库

点击以下网址，打开https://github.com/

进入到仓库页面，新建仓库，可以直接通过https://github.com/doreamon95?tab=repositories，将doreamon95替换为自己的github用户名。或者在github主页登录后点击**右上角头像-Your repositories-**进入到仓库页面。

```
浏览器访问，将doreamon95替换为自己的仓库名
https://github.com/doreamon95?tab=repositories
```

新建仓库，点击屏幕右上方**New**按钮新建仓库，界面如下：

![](https://doreamon95.oss-cn-chengdu.aliyuncs.com/img/001/sgx1574654655553.png)

点击创建仓库，就生成了自己的私有仓库，同样可以在仓库页面看到自己仓库。

## git私有仓库到本地

首先需要注意一点的是，私有仓库git方式和公有仓库不同，比如；https://github.com/doreamon95/go-note.git 这种方式就无法git 仓库下来。正确的git私有仓库方式应该是：

```
git clone  git@github.com:用户名/仓库名.git
```

用过git的人应该都知道，git私有仓库到本地首先是需要进行身份认证的，由于是自己使用，就需要进行SSH key认证，这里我们假设已经进行认证。如果未认证请查看SSH key认证方式。



