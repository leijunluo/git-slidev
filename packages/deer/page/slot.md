# 约定式插槽

通过约定 `组件插槽` 在 `components` 文件夹下的路径，来实现自动注入到组件插槽上。

<div class="grid grid-cols-2 gap-4">
  <span style="opacity: 0.7" class="text-center pb-10px">引入组件</span>
  <span style="opacity: 0.7" class="text-center pb-10px">约定式插槽</span>
</div>

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
import Layout from '@@/components/layout'
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
