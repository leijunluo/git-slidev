# Git 高级用法

```bash
$ git commit --amend

$ git rebase --interactive
$ git rebase --continue
$ git rebase --abort

$ git cherry-pick 
```

<!-- 
amend 命令是修改最近提交的便捷方式。

interactive 命令是交互式变基工具，你可以在任何想要修改的提交后停止，然后修改信息、添加文件或做任何想做的事情。

git rebase -i HEAD~3

continue: 当你修改好了提交信息时，执行 continue 进入下一个修改提交或者退出编辑器。

abort: 放弃 interactive 修改。

注意：已经被推送到远程仓库的提交，不要去修改它的任何信息，提交一个新的修复 commit 上去。

cherry-pick 是从一个分支中选取提交并将其应用到另一个分支的命令。
-->