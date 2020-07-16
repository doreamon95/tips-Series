## 方法一：new 仓库提交

1. 在Github上**new**一个repository；

2. 进入本地的项目目录下，建立**git仓库**：
   git init

3. 将项目所有文件添加到仓库中：
   **git add .** #全部
   git add filename #指定文件

4. 将添加的文件提交到仓库：
   **git commit -m** "文件描述"

5. 将本地仓库**关联**到Github上：
   git remote add origin newrepository_url

6. 同步远程仓库和本地仓库 （远程拉到本地）

   git pull origin master  

7. 上传代码到Github远程仓库（本地到远程）
   git push origin master

##   方法二：远程克隆仓库再提交

​	1. 将远程仓库克隆到本地

​	git clone  git@github.com:用户名/仓库名.git

   2. 查看状态

      git status

   3. 新增文件添加到仓库 或  新增所有添加到仓库

      git add . #全部
      git add filename #指定文件

   4. 添加的文件提交到仓库

      git commit -m  "提交说明"

   5. 查看仓库日志

      git log

   6. 查看仓库状态

      git status

   7. 将本地仓库的内容push到远程仓库

​      git push origin master

## 方法三：私有仓库克隆提交

克隆分为两种情况，私有仓库和公有仓库。如果是私有仓库

```
git clone  git@github.com:用户名/仓库名.git
```

 如果是公有仓库，直接clone到github的链接

```
https://github.com/用户名/仓库名.git
```

### 查看状态git状态

git status

### git提交

首先需要，新增文件添加到仓库 或  新增所有添加到仓库

```bash
git add . #全部
git add filename #指定文件
```

文件添加好之后，需要添加的文件提交到仓库

```bush
git commit -m  "提交说明"
```

可以利用以下命令来查看仓库日志和查看仓库状态

```bush
git log

git status
```

将本地仓库的内容push到远程仓库，其中master为远程仓库分支

```
git push origin master
```

