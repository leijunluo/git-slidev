# 三棵树

- HEAD: 上次提交的快照，下次提交的父结点
- Index: 预期下次提交的快照
- Working: 工作区

<div grid="~ cols-3 gap-6" class="relative mt-10">

<img src="/public/reset-ex1.png" />
<img src="/public/reset-ex2.png" />
<img src="/public/reset-ex3.png" />

</div>

<!--
理解 reset 和 checkout 的最简单方法，就是我们以 Git 的思维框架（将其作为内容管理器）来管理三棵不同的树。

`HEAD` 是当前分支引用的指针，它指向的是当前分支上的最后一次提交。

`Index` 是你的`预期的下一次提交`，其实就是 Git 的 `暂存区`。

`Working` 就是我们的`工作区`。 
-->
