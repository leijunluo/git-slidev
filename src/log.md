
# log

```bash
$ git log
$ git log --graph 
$ git log --oneline
```

# alias

```bash
$ git config --global alias.ci 'log --pretty="format:%C(yellow)%h%C(red)%d\ %C(reset)%s%C(blue)\ [%cn]" --decorate'
$ git config --global alias.ll 'log --pretty=format:"%C(yellow)%h\ %ad%Cred%d\ %Creset%s%Cblue\ [%cn]" --decorate --date=relative'
$ git config --global alias.lds 'log --pretty=format:"%C(yellow)%h\ %ad%Cred%d\ %Creset%s%Cblue\ [%cn]" --decorate --date=short'
$ git config --global alias.lg 'log --graph --pretty=format:"%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset" --abbrev-commit --date=relative --decorate'
```

<!--
ls: 列表以简短的形式提交，带有颜色和分支/标记注释。

ld: 列出相对于当前日期的单行提交 
lds: 列出日期的单行提交。
-->
