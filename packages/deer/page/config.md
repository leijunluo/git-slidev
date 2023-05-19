# 配置文件

<div class="grid grid-cols-2 gap-4">

<div>

- 项目基本配置，例如项目名称、版本、路由等。
- 项目构建配置，例如输出目录、代理、webpack 配置等。
- 插件和功能项的配置。
- 控制某个功能和插件的开与关。

</div>

<div>

- alias <span style="margin-left: 186px">配置别名</span>
- tgz <span style="margin-left: 196px">压缩输出目录</span>
- gzip <span style="margin-left: 186px">构建 gzip 格式</span>
- devServer <span style="margin-left: 140px">本地服务配置</span>
- system <span style="margin-left: 164px">系统配置</span>
- routes、asyncRoutes <span style="margin-left: 52px">基础路由和权限路由</span>

</div>

</div>

<div class="grid grid-cols-2 gap-4 p-22px">

<div>

```js
import routes from './routes';

export default {
  version: '1.0.0-alpha.1',
  system: {
    name: '主体框架',
    code: '1466579472458252289'
  },
  routes,
}
```
</div>

<div>

```js
export default {
  routes: [{
    path: '/',
    component: '@@/components/layout/index',
    routes: [{
      path: '/index',
      component: 'views/about.vue'
    }]
  }]
}
```

</div>

</div>
