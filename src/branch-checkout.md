# branch

```bash
$ git branch --list
$ git branch --all
$ git branch -d iss53
$ git branch 
```

# checkout 

```bash
$ git checkout master
$ git checkout -b iss53
$ git checkout -- path/to/file
```

# switch

```bash
$ git switch <branch>
$ git switch -c <branch>
```

<!--
checkout: 切换分支和恢复工作书文件。

switch: 切换分支。

restore: 恢复工作树中已被修改后的文件。

git push origin --delete dev (删除远程分支或者 tag)

1. 仓库 1
2. 新增 dev 分支
3. 新增 c2.md -> push dev
-->