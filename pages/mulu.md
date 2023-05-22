# 目录结构

```text
├── src
│   ├── cli → 存放cli相关的文档
│   ├── utils → 存放脚本工具相关的文档
│   ├── v2 → 存放Vue2组件的文档
│   ├── v3 → 存放Vue3组件的文档
│   ├── vscodeExtensions → 存放VSCode扩展的文档
│   ├── .vuepress → VuePress 配置文件夹
│   │   ├── dist → 构建输出目录
│   │   ├── components → 该文件夹下的组件会被自动注册，使用方式(<文件名 />, <文件夹名-文件名 />)
│   │   ├── navbar → 顶部导航栏配置文件
│   │   ├── public → 静态资源目录
│   │   │   ├── components → 用于存放vue3/vue2的npm组件，需要是es模式并且除vue外所有的依赖包需要打包进来。
│   │   │   ├──            → 目前不支持app.use()只能使用component的格式。
│   │   │   ├── utils → 工具脚本，可以在md文件中使用importmap引入
│   │   ├── styles → 用于存放样式相关的文件
│   │   ├── config.ts → 配置文件的入口文件
│   │   ├── client.ts → 客户端文件
│   │   ├── theme.ts → 主题配置文件
```
