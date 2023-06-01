# 插件

插件机制是 deer 的核心之一，通过它我们可以灵活扩展功能，同时保证应用的可维护性。

* 提供丰富的生命周期
* 提供丰富插件 API
* 插件分为 plugin 和 preset 两种类型
* 自动扫描项目插件依赖并注册

<div class="pt-10"></div>

```ts
// @deer/plugin-alias-api
import { IApi } from 'deer'

export default (api: IApi) => {
  api.chainWebpack((memo) => {
    memo.resolve.alias.set('api', './apis')
  })
}
```
