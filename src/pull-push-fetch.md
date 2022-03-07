# fetch

```bash
$ git fetch
```

# pull

```bash
$ git pull
$ git pull <remote>
```

# push

```bash
$ git push
$ git push origin master
$ git push origin HEAD
$ git push -u origin HEAD
```

<!-- 
fetch: 从远程存储库中下载对象和分支引用。 

push HEAD: push 时不需要指定分支名称了，默认使用的是当前分支名称。

-u push HEAD: 在推送的同时设置当前分支为默认分支，供其他命令使用。比如：pull、push 等。
-->
