# reset

```bash
$ git reset --soft HEAD~
$ git reset --mixed HEAD~
$ git reset --hard HEAD~
```

<div grid="~ cols-3 gap-6" class="relative mt-10">

<img src="/public/reset-soft.png" />
<img src="/public/reset-mixed.png" />
<img src="/public/reset-hard.png" />

</div>

<!-- 
`soft` 将上次 `commit` 撤销到暂存区。

`mixed` 将上次 `commit` 撤销到工作目录。reset 默认是 mixed。

`hard`: hard 是 reset 命令唯一的危险用法，它会强制覆盖当前的工作目录。在这种特殊情况下，我们的 Git 数据库中的一个提交内还留有该文件的 v3 版本， 我们可以通过 reflog 来找回它。但是若该文件还未提交，Git 仍会覆盖它从而导致无法恢复。
-->