# push

```bash
$ git push
$ git push origin master
$ git push origin HEAD
$ git push -u origin HEAD
```

# pull

```bash
$ git pull
$ git pull <remote>
```

<!-- 
fetch: 从远程存储库中下载对象和分支引用。 

push HEAD: push 时不需要指定分支名称了，默认使用的是当前分支名称。

-u push HEAD: 在推送的同时设置当前分支为默认分支，供其他命令使用。比如：pull、push 等。

1. `git remote add origin <URL>` 
2. git push origin master
3. 新建一个本地仓库 (mkdir ../git-ppt-2)
4. 仓库 2 pull
-->
