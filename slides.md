---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# page transition
transition: slide-left
# use UnoCSS
css: unocss
hideInToc: true
---

# 文档系统介绍

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
  </span>
</div>

#### 本文档系统是基于 [vuepress](https://v2.vuepress.vuejs.org/zh/)、[vuepress-theme-hope](https://theme-hope.vuejs.press/zh/)完成的
<div class="mt5"></div>

#### [仓库地址](http://gitlab.ilabpower.devops/neotrident/fe-wiki)
<div class="mt5"></div>

#### [在线演示](https://ynqq.github.io/doc/)

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
src: ./pages/mulu.md
---
---
src: ./pages/shiyong.md
---
---
src: ./pages/mokuai.md
---
---
src: ./pages/vue.md
---
---
src: ./pages/js.md
---
---
src: ./pages/buzu.md
---

