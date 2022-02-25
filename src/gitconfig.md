# gitconfig

Git 自带一个 git config 的工具来帮助设置控制 Git 外观和行为的配置变量。 这些变量存储在三个不同的位置

- **系统** - /etc/gitconfig: 包含系统上每一个用户及他们仓库的通用配置。
- **用户** - ~/.gitconfig 或 ~/.config/git/config 文件：只针对当前用户。
- **本地** - 当前使用仓库的 Git 目录中的 config文件（即 .git/config）：针对该仓库。

## 常用命令

```ts
$ git config --global user.name luoleijun

$ git config --global user.email luoleijun@gmail.com

$ git config —list

$ git config user.name
```
