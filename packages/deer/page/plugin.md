# 插件开发

增加 Webpack alias 配置

```ts
import { IApi } from 'deer'

export default (api: IApi) => {
  api.chainWebpack((memo) => {
    memo.resolve.alias.set('api', './api')
  })
}
```
