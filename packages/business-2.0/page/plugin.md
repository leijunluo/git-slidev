# 插件开发

增加 Webpack alias 配置

```ts
import { IApi } from 'business'

export default (api: IApi) => {
  api.chainWebpack((memo) => {
    memo.resolve.alias.set('api', './api')
  })
}
```
