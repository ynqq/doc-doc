# 脚本工具代码演示
- 使用方式:
1. 将dist文件复制到文档的 public/utils 文件夹下
2. 在md文件中的【imports】中引入  
    - 如果工具引入了第三方包需要判断是什么类型的  
        1. es文件 需要引入第三方包的es文件
        2. umd文件 需要引入第三方包带有全局变量的包,然后用initScript方法引入
3. 编写对应的案例代码

<Transform :scale=0.5 class="absolute -right-40 top-10">
@2

````json
@import
\`\`\`json
{
  "imports": {
    "moment": "https://unpkg.com/moment@2.29.4/src/moment.js",
    "momentTest": "/utils/momentTest/index.js"
  }
}
\`\`\`
````

</Transform>
<Transform :scale=0.5 class="absolute right-0 top-50">
@3

````js
<script setup>
import {getNowDate} from 'momentTest'
const log = () => {
  console.log(getNowDate());
};
</script>

<template>
  <div @click="log">获取当前日期
  </div>
</template>
````

</Transform>