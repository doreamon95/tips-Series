

## 问题1

输入 `git remote add origin https://github.com/username/yourrepository.git`

提示：fatal: remote origin already exists

解决

```
git remote rm origin
```

然后再次输入

```
git remote add origin https://github.com/username/yourrepository.git
```

## 问题2

输入`git push origin master`

提示 error:failed to push som refs to

解决，将远程拉到本地，再提交

```
git pull origin master
git push origin master
```

### 问题3

出现Could not read from remote repository

输入

```
git remote add origin https://github.com/username/yourrepository.git
```



