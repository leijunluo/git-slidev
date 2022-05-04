# 中间件开发

中间件是你想要在实例化 Vue 应用程序之前运行的 JavaScript 插件。

`middleware` 是中间件存目录。中间件

```ts
// middleware/router-login.js

export default ({ router, $auth}) => {
  const { getToken } = $auth

  router.beforeEach((_to, _from, next) => {
    if(to.name !== 'Login' && !getToken()) {
      next({ name: 'Login' })
    } else {
      next()
    }
  })
}
```
