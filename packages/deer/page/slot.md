# 约定式插槽

约定式插槽就是通过约定 `插槽组件` 在 `components` 文件夹下的路径，来实现自动注入到组建内部插槽上。

<div class="grid grid-cols-2 gap-4">

```vue
<template>
  <layout>
    <template v-slot:footer>
      底部信息栏～～～
    </template>
  </layout>
</template>
<script>
  import Layout from '@business/component-layout'
  export default {
    components: { Layout }
  }
</script>
```

```vue
// components/_layout/footer/index.vue
<template>
  通过约定式插槽注入到底部信息栏～～～
</template>
```
</div>
