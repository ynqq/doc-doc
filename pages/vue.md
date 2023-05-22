# Vue 组件代码演示

- [theme-hope Vue交互演示地址](https://theme-hope.vuejs.press/zh/guide/markdown/vue-playground.html)
- 这个功能是 theme-hope 集成[@vue/repl](https://github.com/vuejs/repl)实现的
- 使用方式:
  1. 单独打包一份除了 vue 之外的完整包
  2. 将 es 文件和 css 复制到文档的 public/component 文件夹下使用
  3. 在 md 文件中的【imports】中引入
  4. 引入对应的样式和组件

<Transform :scale=0.5 class="absolute -right-40 top-10">
@3

````json
@import
\`\`\`json
{
  "imports": {
    "Com": "/components/v3/neo-custom-form-next/index.es.js",
    "utils": "/utils/index.js"
  }
}
\`\`\`
````

</Transform>
<Transform :scale=0.5 class="absolute -right-50 top-50">
@4

````js
<script setup>
import { ref } from "vue"; // vue是 @vue/repl 自带的 可以直接引用
import { CustomForm } from "Com"; // 引入组件 不支持插件
import { initStyle } from "utils";// 加载组件样式的脚本
initStyle("/components/v3/neo-custom-form-next/style.css"); // 加载组件样式
const list = ref([]);
const log = () => {
  console.log(list.value);
};
</script>

<template>
  <div>
    <button @click="log">获取数据</button>
    <CustomForm v-model:value="list" />
  </div>
</template>
````

</Transform>
