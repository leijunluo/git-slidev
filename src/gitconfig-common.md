# 通用配置

## 用户信息

```bash
$ git config --global user.name luoleijun
$ git config --global user.email luoleijun@gmail.com
```

## alias

```bash
$ git config --global alias.ci commit
$ git config --global alias.co checkout
$ git config --global alias.br branch
$ git config --global alias.st status
$ git config --global alias.pl pull
$ git config --global alias.ps push
```

## 其他

```bash
$ git config --global fetch.prune true
$ git config --global pull.rebase true
```

<!-- 
fetch.prune: 每次您从远程获取更改时，将会自动清除在本地存储库中的Git 对象。

pull.rebase: pull 默认是使用 merge 行为从远程仓库拉取 commit。
-->
