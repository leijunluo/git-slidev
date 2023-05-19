# 请求

在请求类型前面加 $ 符号使用的是 Business 针对于 axios 封装的规则。post 请求需要加 form 格式，在请求类型后面加 Form（$postForm）。

<div class="grid grid-cols-[160px_1fr_1fr] gap-x-3 pb-10px">
  <span></span>
  <span class="ml-16px" style="opacity: 0.7">Business</span>
  <span class="ml-16px" style="opacity: 0.7">deer</span>
</div>

<div class="grid grid-cols-[160px_1fr_1fr] gap-x-3">

<span style="opacity: 0.8">步骤</span>

<img class="h-16" src="business-axios.png"/>

<img class="h-16" src="deer-axios.png"/>
</div>

<hr style="opacity: 0.8" class="mt-10px" />

<div class="grid grid-cols-2 pt-20px">

<div class="pr-2">

```js
// apis/menu.js

export default ({ $get, $post }) => {
  return {
    getMenu: (params) => {
      return $get('/manage/v1/getMenu', params)
    },
    getMenuItem: (params) => {
      return $post('/manage/v1/getMenuItem', params)
    }
  }
}
```

</div>

<div class="pl-2 h-300px">

```vue
<script>
export default {
  async mounted() {
    const { data } = await this.$apis.menu.getMenu({ 
      id: '1934123221452' 
    })
  }
}
</script>
```

</div>

</div>
