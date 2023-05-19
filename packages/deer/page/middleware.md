# 中间件

中间件是在渲染页面或路由前执行的函数。中间件可以用于许多场景，比如身份验证、路由前的数据处理等。

<div class="grid grid-cols-2 gap-4 mt-40px">
  <span style="opacity: 0.7" class="text-center pb-10px">登录状态</span>
  <span style="opacity: 0.7" class="text-center pb-10px">添加函数到 Context</span>
</div>

<div class="grid grid-cols-2 gap-4">

```js
// middleware/router-login.js
export default ({ router, $auth }) => {
  const { loggedIn } = $auth
  
  router.beforeEach((to, _form, next) => {
    // 如果用户未登录并且路由不是 Login，则跳转到登录页面
    if (!loggedIn && to.name !== 'Login') {
      next({ name: 'Login' })
    } else {
      next()
    }
  })
}
```

```js
// middleware/hello.js

export default (_, inject) => {
  inject('hello', msg => console.log(`hello ${msg}!`))
}
```

</div>
