# 目录结构

<div class="grid grid-cols-2 gap-4">
  <span style="opacity: 0.7" class="text-center pb-10px">Business</span>
  <span style="opacity: 0.7" class="text-center pb-10px">deer</span>
</div>

<div class="grid grid-cols-2 gap-4">

```
├── dist                    // 打包输出目录
├── public           
│   └── favicon.ico         // 项目图标
├── src              
│   ├── .deer               // 临时文件目录
│   ├── .deer-production    // 临时文件目录
│   ├── apis                // 接口
│   ├── assets              // 静态资源
│   ├── components          // 组件和约定式插槽
│   ├── middlewares         // 中间件
│   ├── store               // Vuex store
│   ├── svgs                // svg 资源
│   ├── views               // 业务代码
│   └── main.js             // 入口文件
├── .deerrc.js              // deer 配置文件
├── .eslintignore           // ESLint 文件屏蔽
├── .eslintrc.js            // ESLint 配置项
├── .girignore              // git 文件屏蔽
└── package.json            // 依赖管理
```

```bash
├── assets/       // 存放静态资源文件，如 CSS、图片等
├── components/   // 存放 Vue 组件
├── layouts/      // 存放页面布局组件
├── middleware/   // 存放中间件
├── pages/        // 存放页面，页面对应路由路径
├── plugins/      // 存放插件文件
├── static/       // 存放静态文件，如 favicon.ico
├── store/        // 存放 Vuex 状态管理文件
├── nuxt.config.js // Nuxt.js 配置文件
└── package.json  // 项目依赖及配置文件
```
</div>
