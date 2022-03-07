
# log

```bash
$ git log
$ git log --graph 
$ git log --stat
$ git log --shortstat
$ git log --name-status
$ git log --oneline
$ git log --pretty="format:%C(yellow)%h%C(red)%d\\ %C(reset)%s%C(blue)\\ [%cn]" --decorate
$ git log --pretty=format:"%C(yellow)%h\\ %ad%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate --date=relative
$ git log --pretty=format:"%C(yellow)%h\\ %ad%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate --date=short
$ git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative --decorate
```

<!--
ls: 列表以简短的形式提交，带有颜色和分支/标记注释。

ld: 列出相对于当前日期的单行提交 
lds: 列出日期的单行提交。
-->
