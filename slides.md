---
css: unocss
layout: cover
colorSchema: dark
highlighter: shiki
transition: fade-out
---

<script setup>
import { toggleDark } from "vue-dark-switch"

toggleDark(true)
</script>

<h1 flex="~ col">
<div>tov-template</div>
<div>开箱即用现代开发模板</div>
<div>vite + vue3 + ts</div>
</h1>

<a uppercase text-sm tracking-widest href="https://github.com/markthree" target="__blank">
markthree
</a>

<img src="/tov-template/logo.png" w-40 abs-tr mt-30 mr-20 />

<div abs-br mx-10 my-12 flex="~" items-center text-sm text-right>

 <carbon-logo-github class="inline-block" mr-2 /> <a href="https://github.com/dishait/tov-template" target="__blank">github.com/dishait/tov-template</a>

</div>


---

<div text-lg op50 mb-4>动机</div>

## 为什么要开发 `tov-template` 模板?

<div text-2xl mt-10>
<v-clicks>

- 为了项目<span text-red-500>更易维护</span>，统一代码规范和风格

- 下次开发直接用，<span text-red-500>节省时间</span>，不需要重新配置
  
- 整合主流插件搭建现代开发架构，<span text-red-500>提高开发效率</span>

</v-clicks>
</div>

<carbon-fire text-15vw abs-tr mt-10 mr-10 />


---
layout: two-cols
class: 'px-2'
---


<template v-slot:default>

<v-clicks>

# 现状

> 现在怎么样?

</v-clicks>

<div mt-6 flex="~ col" space-y-8>
  <v-clicks>
      <span flex="~ gap-2" items-center>
         <carbon-time /> <code>2022/1/8</code> 起开源至今
      </span>
      <span flex="~ gap-2" items-center>
         <carbon-star /> <code>524</code> star，<code>134</code> fork
      </span>
      <span flex="~ gap-2" items-center>
         <carbon-reference-architecture /> <code>369</code> 次 commit，<code>36</code> 个 feature
      </span>
  </v-clicks>
</div>

</template>

<template v-slot:right>

<v-clicks>

# 方向

> 一直以来的方向

</v-clicks>

<div mt-6 flex="~ col" space-y-8>
   <v-clicks>
      <span flex="~ gap-2" items-center>
         <carbon-uv-index />好的开发体验 → <code>DX</code>
      </span>
      <span flex="~ gap-2" items-center>
         <carbon-chemistry /> 通用但面向现代 → <code>universal</code>
      </span>
      <span flex="~ gap-2" items-center>
         <carbon-volume-block-storage /> 尽量的开箱即用 → <code>out-of-the-box</code>
      </span>
   </v-clicks>
</div>
</template>


---
layout: center 
growX: 50 
growY: 50
---


<Badge :value="36"><h1 font-bold class="text-5xl! text-white">特性</h1></Badge>

<div absolute left-100 top-80 v-click>vite</div>
<div absolute left-52 top-50 v-click>vue3</div>
<div absolute left-100 top-50 v-click>pnpm</div>
<div absolute left-50 top-80 v-click>文件路由</div>


<div absolute left-140 top-50 v-click>布局系统</div>
<div absolute left-145 top-80 v-click>mock</div>
<div absolute left-170 top-80 v-click>api 自动引入</div>
<div absolute left-60 top-90 op80 v-click>组件自动引入</div>
<div absolute left-90 top-90 v-click>图标自动引入</div>

<div absolute left-85 top-40 v-click>vueuse</div>
<div absolute left-130 top-90 v-click>typescript</div>
<div absolute left-125 top-40 op70 v-click>unocss</div>
<div absolute left-55 top-40 op70 v-click>暗黑模式</div>
<div absolute left-170 top-50 op70 v-click>swr</div>


<div absolute left-145 top-100 op60 v-click>pinia</div>
<div absolute left-100 top-30 op70 v-click>跳转进度条</div>
<div absolute left-70 top-30 op70 v-click>开发面板</div>
<div absolute left-130 top-30 op70 v-click>插件自动加载</div>
<div absolute left-120 top-100 op70 v-click>vitest</div>
<div absolute left-70 top-100 op60 v-click>markdown 渲染</div>


<div absolute left-170 top-90 op60 v-click>路径别名 <code>~</code></div>
<div absolute left-100 top-20 op70 v-click>命令行自动创建与删除</div>
<div absolute left-70 top-50 op70 v-click>i18n 国际化</div>
<div absolute left-160 top-40 op70 v-click>漂亮的 404 页</div>
<div absolute left-130 top-80 op70 v-click>tsx</div>
<div absolute left-80 top-80 op60 v-click>gzip</div>

<div absolute left-35 top-98 op60 v-click>环境变量配置</div>
<div absolute left-100 bottom-20 op70 v-click>统一的代码规范和风格</div>
<div absolute left-155 top-18 op50 v-click>生产环境自动移除开发日志</div>
<div absolute left-170 top-26 op70 v-click>defineOptions</div>
<div absolute left-180 bottom-30 op70 v-click>echarts</div>
<div absolute left-150 top-66 op60 v-click>全局通用 toast</div> 
<div absolute left-44 top-65 op60 v-click>全局通用 axios 请求封装</div>
<div absolute left-30 bottom-18 op60 v-click>自动生成环境变量类型声明</div> 
<div absolute left-50 top-18 op70 v-click>renovate 自动更新依赖</div> 
<div absolute left-150 bottom-18 op50 v-click>自动版本更新并生成 CHANGELOG</div>   


---
layout: 'center' 
class: 'text-center' 
growX: 50 
growY: 10
---

<div v-click transition-all duration-500 :class="$slidev.nav.clicks === 0 ? 'op0' : $slidev.nav.clicks > 1 ? 'op50 text-2xl' : 'translate-y-10 text-4xl'">介绍</div>

<div v-click>
  <h1>特性</h1>
</div>


---
layout: two-cols
class: px-2
---

# <logos-vitejs text-md /> vite

> 下一代的前端工具链

<div my-2>
<v-clicks>

- 超快的 `hmr`

- 极速的服务启动 - esbuild

- 配置简单，容易扩展 - rollup

</v-clicks>
</div>

<v-clicks>

<div mt-20 space-y-5>

<carbon-link text-sm /> [cn.vitejs.dev/guide/why · 为什么选 Vite?](https://cn.vitejs.dev/guide/why.html)

</div>

</v-clicks>

::right::

<v-clicks>

# QA

> 如何加快 `vite` 冷启动?

</v-clicks>

<div my-2>
<v-clicks>

- 更新 `vite` 版本为 [4.3.0](https://github.com/vitejs/vite/blob/v4.3.9/packages/vite/CHANGELOG.md#430-2023-04-20) 以上 

- 安装预热转换插件 <Repo class="text-sm" name="bluwy/vite-plugin-warmup" text-red-200 />

```ts
// vite.config.ts
import { warmup } from 'vite-plugin-warmup'

export default defineConfig({
   plugins: [
      warmup({ clientFiles: ['./src/**/*'] }) // 预热
   ]
})
```

</v-clicks>
</div>


---
layout: two-cols
class: px-2
---

# <logos-vue text-md /> vue3

> 相比 vue2

<div my-2>
<v-clicks>

- 更快的渲染

- 组合式 `api`

- 更小的 `bundle`

- `TypeScript` 友好

</v-clicks>
</div>
<v-clicks>

<div mt-20 space-y-5>

<carbon-link text-sm /> [v3-migration.vuejs.org/zh · vue 3 迁移指南](https://nuxt.com.cn/docs/guide/concepts/vuejs-development#%E4%B8%8Enuxt2-vue2%E7%9A%84%E5%8C%BA%E5%88%AB)

</div>

</v-clicks>

::right::

<v-clicks>

# Usage

> 如何在 `vite` 中使用？

</v-clicks>

<div my-2>
<v-clicks>

- SFC 单文件组件支持  <Repo class="text-sm" name="@vitejs/plugin-vue" text-red-200 />

```ts
// vite.config.ts
import Vue from '@vitejs/plugin-vue'

export default defineConfig({
   plugins: [Vue()]
})
```

```html
<script setup>
import { ref } from "vue"

const count = ref(1)
</script>

<template>
   <button @click="count++">{{ count }}</button>
</template>
```

</v-clicks>
</div>


---
layout: two-cols
class: px-2
---

# <logos-pnpm text-md /> pnpm

> 一个依赖管理器，相比 `npm` 和 `yarn`

<div my-2>
<v-clicks>

- 没有幽灵依赖

- 支持 `monorepos` 

- 比其他包管理器快 `2` 倍
  
</v-clicks>
</div>
<v-clicks>

<div mt-20 space-y-5>

<carbon-link text-sm /> [pnpm.io/zh · pnpm 官网](https://pnpm.io/zh/)

</div>

</v-clicks>

::right::

<v-clicks>

# Usage

> 如何使用？

</v-clicks>

<div my-2 space-y-2>
<v-clicks>

1. 安装 `pnpm`

```shell
npm i pnpm -g
```

2. 安装依赖

```shell
pnpm i # npm install
```

3. 安装对应依赖

```shell
pnpm i vue # npm install vue
```

</v-clicks>
</div>


---

# <carbon-3d-curve-auto-colon text-md /> 文件路由

> 目录结构即路由

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="posva/unplugin-vue-router" text-red-200 />

</v-clicks>

<div my-2>
<v-clicks>

- `src/pages/index.vue` => `/`
- `src/pages/about.vue` => `/about`
- `src/pages/users/[id].vue` => `/users/:id`

- `src/pages/users/index.vue` => `/users`
- `src/pages/users/profile.vue` => `/users/profile`
- `src/pages/[user]/settings.vue` => `/:user/settings`

- `src/pages/[...notFound].vue` => 404 路由
  
</v-clicks>
</div>

---

# <carbon-3d-curve-manual text-md /> <Badge :value="1" class="text-white">布局系统</Badge>


<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="dishait/vite-plugin-vue-meta-layouts" text-red-200 />

</v-clicks>


<v-clicks>


<div text-white>

   `src/layouts/default.vue` 将作为默认布局

</div>


```html
<!-- src/layouts/default.vue -->
<template>
	我是默认布局
	<router-view />
	<!-- 页面视图出口 -->
</template>
```

</v-clicks>


<div grid-cols-2 grid gap-4>

<div>

<v-clicks>

此时 `src/pages/index.vue`

```html
<!-- src/pages/index.vue -->
<template>
	<div>我是首页</div>
</template>
```

路由到 `/`时，页面将渲染

```html
我是默认布局 我是首页
```

</v-clicks>


</div>


<div>

<v-clicks>

此时 `src/pages/about.vue`

```html
<!-- src/pages/about.vue -->
<template>
	<div>我是关于页</div>
</template>
```

路由到 `/about` 时，页面将渲染

```html
我是默认布局 我是关于页
```

</v-clicks>

</div>

</div>



---
layout: two-cols
class: px-2
---

# <carbon-3d-curve-manual text-md /> <Badge :value="2" class="text-white">布局系统</Badge>


<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="dishait/vite-plugin-vue-meta-layouts" text-red-200 />

</v-clicks>


#### 非默认布局

随便创建一个 `src/layouts/custom.vue`

```html
<!-- src/layouts/custom.vue -->
<template>
	我是非默认布局custom
	<router-view />
	<!-- 页面视图出口 -->
</template>
```

::right::


<div mt-16></div>

<v-clicks>

此时 `src/pages/index.vue` 内

```html
<!-- src/pages/index.vue -->
<template>
	<div>我是首页</div>
</template>

<!-- 添加自定义块 👇 -->
<route lang="json">
{
	"meta": {
		"layout": "custom"
	}
}
</route>
```

此时路由到 `/`, 页面将渲染

```html
我是非默认布局custom 我是首页
```

</v-clicks>


---
layout: two-cols
class: px-2
---

# <carbon-virtual-private-cloud-alt text-md pt-1 /> <Badge :value="1" class="text-white">api 自动引入</Badge>

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="antfu/unplugin-auto-import" text-red-200 />

</v-clicks>

<v-clicks>

<div>

原本 `vue` 的 `api` 需要自行 `import`。

</div>

```ts
import { computed, ref } from "vue";
const count = ref(0);
const doubled = computed(() => count.value * 2);
```

现在可以直接使用，而且是按需自动引入的。

```ts
const count = ref(0);
const doubled = computed(() => count.value * 2);
```

</v-clicks>

::right::

<div mt-15 v-click>

目前模板支持自动引入 `api` 的库列表

- `vue`
- `vuex`
- `pinia`
- `vue-i18n`
- `vue-router`
- `@vueuse/core`
- `@vueuse/head`
- `@vueuse/math`
  
只要确保项目已经安装上述依赖即可用

</div>


---

# <carbon-virtual-private-cloud-alt text-md pt-1 /> <Badge :value="2" class="text-white">api 自动引入</Badge>

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="antfu/unplugin-auto-import" text-red-200 />

</v-clicks>

<v-clicks>

<div mb-15>

当然还有本地目录地自动引入，只需要满足以下规范即可

`src` 下的 `composables`，`store` 和 `api` 的模块导出将被按需自动引入

</div>


例如有个 `src/composables/foo.ts`

```ts
// default 导出
export default 1000;
```

此时就不再需要 `import`了

```html
<script setup lang="ts">
	console.log(foo) // 输出 1000
</script>
```

</v-clicks>


---
layout: two-cols
class: px-2
---

# <carbon-app-connectivity text-md pt-1 /> <Badge :value="1" class="text-white">组件自动引入</Badge>

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="antfu/unplugin-vue-components" text-red-200 />

</v-clicks>

<v-clicks>

<div>

原来需要 `import`

</div>

```html
<script setup lang="ts">
	import Hello from '../components/Hello.vue'
</script>

<template>
	<Hello />
</template>
```

现在在 `src/components` 下的组件都会被按需引入

```html
<template>
	<Hello />
</template>
```

</v-clicks>

::right::

<div mt-15 v-click>

当然也支持嵌套组件，例如 `src/components/foo/bar.vue` 👇

```html
<template>
	<FooBar />
</template>
```

</div>


---
layout: two-cols
class: px-2
---

# <carbon-app-connectivity text-md pt-1 /> <Badge :value="2" class="text-white">组件自动引入</Badge>

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="antfu/unplugin-vue-components" text-red-200 />

</v-clicks>



<div mb-15>

<v-clicks>

<span text-red-400>流行的组件库支持</span>

只需安装依赖，无需配置

例如 [naive-ui](https://github.com/tusen-ai/naive-ui)，只需安装依赖

```shell
pnpm add naive-ui
```

即可在模板中使用

```html
<!-- src/pages/index.vue -->
<template>
	<n-button type="success">Success</n-button>
</template>
```

</v-clicks>

</div>


::right::

<div mt-15 v-click>

   目前支持的组件库有

</div>

<div flex space-x-10 v-click>

<div>

- [vant](https://github.com/youzan/vant)
- [idux](https://github.com/IDuxFE/idux)
- [devui](https://github.com/DevCloudFE/vue-devui)
- [quasar](https://github.com/quasarframework/quasar)
- [varlet](https://github.com/varletjs/varlet)
- [inkline](https://github.com/inkline/inkline)
- [vuetify](https://github.com/vuetifyjs/vuetify)
- [@headlessui/vue](https://github.com/tailwindlabs/headlessui)
- [tdesign-vue-next](https://github.com/Tencent/tdesign-vue-next)

</div>


<div>

- [naive-ui](https://github.com/TuSimple/naive-ui)
- [primevue](https://github.com/primefaces/primevue)
- [layui-vue](https://gitee.com/layui/layui-vue)
- [view-design](https://iviewui.com/)
- [arco-design](https://github.com/arco-design/arco-design)
- [element-plus](https://github.com/element-plus/element-plus)
- [ant-design-vue](https://github.com/vueComponent/ant-design-vue)
- [@vueuse/components](https://github.com/vueuse/vueuse/tree/main/packages/components)

</div>

</div>


---
layout: two-cols
class: px-2
---

# <carbon-plug text-md pt-1 /> 插件自动安装

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="dishait/vite-plugin-use-modules" text-red-200 />

</v-clicks>

<v-clicks>

<div>

以前我们需要手动 `use` 来安装 `vue` 插件 

</div>

```ts{1-4|5-8|7-11}
import App from './App.vue'
import { createApp } from "vue"
import { createPinia } from "pinia"

const app = createApp(App)
const pinia = createPinia()

// pinia 做一些操作，省略 n 行代码 ....

app.use(pinia) // 手动 use 安装插件

app.mount('#app')
```

</v-clicks>

::right::

<div mt-15 v-click>

现在只要 `src/plugins` 下模块默认导出 `vue` 插件就会被自动安装

```ts
// src/plugins/pinia.ts
import { createPinia } from "pinia"

// pinia 做一些操作，省略 n 行代码 ....

const pinia = createPinia()

export default pinia // 默认导出的插件，将被自动安装
```

</div>



---

# <logos-vueuse text-md pt-1 /> vueuse

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="vueuse/vueuse" text-red-200 />

</v-clicks>


<v-clicks>

一个超级强的组合式函数库，例如你要获取鼠标位置，只需要这样 👇

```html
<script setup lang="ts">
	// useMouse 被自动按需引入了，不需要import
	const { x, y } = useMouse()
</script>

<template>
	<div>x坐标 {{x}}</div>
	<div>y坐标 {{y}}</div>
</template>
```

</v-clicks>



---

# <logos-typescript-icon text-md pt-1 /> TypeScript 友好的

<v-clicks>

<div>

不需要重新配置，直接可以用 `ts` 书写

</div>

```ts
// src/composables/foo.ts
interface Foo {
   bar: number
}

const foo: Foo = { bar: 1 }
```

或者 `SFC` 单文件组件上加 `lang="ts"` 来支持 `ts`

```vue
<script setup lang="ts">
interface Bar { 
   foo: number
}

const bar: Bar = { foo: 2 }
</script>
```

</v-clicks>


---

# <logos-unocss text-md pt-1 /> <Badge :value="1" dark:text-white text-dark>unocss</Badge>

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="unocss/unocss" text-red-200 />

</v-clicks>


<v-clicks>

即时按需的 `原子css` 引擎。

```html
<template>
	<div class="bg-red-500 text-white">我是红色背景的白色文本</div>
</template>
```

上述模板将渲染红色背景白色的字。

同时支持
[属性化模式](https://cn.windicss.org/features/attributify.html#attributify-mode)，即可以用简写。

```html
<template>
	<div text="white" bg="red-500">我是红色背景的白色文本</div>
</template>
```

这在调整边距尺寸以及等方面可以减少代码量


<div mt-20 space-y-5>

<carbon-link text-sm /> [antfu.me/posts/reimagine-atomic-css-zh · 重新构想原子化CSS](https://antfu.me/posts/reimagine-atomic-css-zh)

</div>


</v-clicks>


---

# <logos-unocss text-md pt-1 /> <Badge :value="2" dark:text-white text-dark>unocss</Badge>

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="unocss/unocss" text-red-200 />

</v-clicks>


<v-clicks>

## <Badge :value="1" type="success" dark:text-white text-dark>图标自动引入</Badge>

前往  [icones.netlify.app](https://icones.netlify.app/) 复制

<script setup lang="ts">
import { NCarousel } from "naive-ui"
</script>


 <n-carousel
    direction="vertical"
    dot-placement="right"
    show-arrow
    mousewheel
    style="width: 100%; height: 240px"
  >
    <img
      class="carousel-img"
      src="/tov-template/icons-first-step.png"
    >
    <img
      class="carousel-img"
      src="/tov-template/icons-second-step.png"
    >
    <img
      class="carousel-img"
       src="/tov-template/icons-third-step.png"
    >
  </n-carousel>


<style scoped>
.carousel-img {
  width: 100%;
}
</style>

点击复制图标名称

</v-clicks>

---

# <logos-unocss text-md pt-1 /> <Badge :value="3" dark:text-white text-dark>unocss</Badge>


<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="unocss/unocss" text-red-200 />

</v-clicks>


<v-clicks>

## <Badge :value="2" type="success" dark:text-white text-dark>图标自动引入</Badge>

在模板中即可通过 `class` 的方式直接使用，注意加上前缀 `i-`。

```html
<template>
	<div class="i-mdi:account-box-multiple"></div>
</template>
```


<div mt-20 space-y-5>

<carbon-link text-sm /> [antfu.iconify · vscode 图标插件](https://marketplace.visualstudio.com/items?itemName=antfu.iconify)

</div>


</v-clicks>



---
layout: two-cols
class: px-2
---


# <line-md-sunny-outline-to-moon-alt-loop-transition text-md pt-1 /> <Badge :value="1" dark:text-white text-dark>暗黑模式</Badge>

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="dishait/vue-dark-switch" text-red-500 dark:text-red-200 />

</v-clicks>

<v-clicks>

## 组件

<!-- 引入 switch，ppt 效果 -->
<script setup lang="ts">
import { SwitchIcon, Switch } from 'vue-dark-switch'
</script>

<div flex items-center mt-2>
   <div mr-2>Switch</div><Switch />
</div>

```html
<script setup lang="ts">
import { Switch } from 'vue-dark-switch'
</script>

<template>
	<Switch />
</template>
```

<div flex items-center mt-3>
   <div mr-2>SwitchIcon</div><SwitchIcon />
</div>

```html
<script setup lang="ts">
import { SwitchIcon } from 'vue-dark-switch'
</script>

<template>
	<SwitchIcon />
</template>
```

</v-clicks>

::right::

<div mt-15>

<v-clicks>

<div flex items-center mt-2>
   <div mr-2>自定义图标</div>
   <SwitchIcon text-lg>
   <template #dark>
      <carbon-partly-cloudy-night /> 
   </template>
   <template #light>
     <carbon-light />
   </template>
</SwitchIcon>
</div>


```html
<script setup>
import { SwitchIcon } from 'vue-dark-switch'
</script>

<template>
	<SwitchIcon>
		<template #dark>
			<i-carbon:partly-cloudy-night  />
		</template>
		<template #light>
			<i-carbon:partly-cloudy-night  />
		</template>
	</SwitchIcon>
</template>
```

</v-clicks>

</div>



---
layout: two-cols
class: px-2
---


# <line-md-sunny-outline-to-moon-alt-loop-transition text-md pt-1 />  <Badge :value="2" dark:text-white text-dark>暗黑模式</Badge>

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="dishait/vue-dark-switch" text-red-500 dark:text-red-200 />

</v-clicks>

<v-clicks>

## 手动

```ts
import { isDark, toggleDark } from "vue-dark-switch";

isDark.value; // 是否是暗黑模式

toggleDark(false); // 取消暗黑模式

toggleDark(true); // 开启暗黑模式

toggleDark(); // 切换模式
```

</v-clicks>

::right::

<div mt-15>

<v-clicks>

## naive ui 支持


```html
<!-- App.vue -->
<script setup>
import { NConfigProvider } from 'naive-ui'
import { naiveTheme } from 'vue-dark-switch'
// naiveTheme 会是完全自动的
</script>

<template>
	<n-config-provider :theme="naiveTheme"> 
      <router-view /> 
   </n-config-provider>
</template>
```

</v-clicks>

<script setup lang="ts">
import { NButton, NConfigProvider } from "naive-ui"
import { naiveTheme, SwitchIcon } from 'vue-dark-switch'
</script>

<div flex items-center mt-5 justify-evenly v-click>


<SwitchIcon />

<n-config-provider :theme="naiveTheme"> 
      <n-button>naive button</n-button>
</n-config-provider>

</div>

</div>


---

# <carbon-progress-bar text-md /> 跳转进度条

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="rstacruz/nprogress" text-red-500 dark:text-red-200 />



跳转进度条由 `nprogress` 实现，可在 `src/styles/main.css` 中调整配色。


```css{|5}
/** src/styles/main.css **/

/** 省略其他样式 **/
#nprogress .bar {
	@apply bg-blue-700 bg-opacity-75; /** 配色 **/

	position: fixed;
	z-index: 1031;
	top: 0;
	left: 0;

	width: 100%;
	height: 2px;
}
```

`@apply` 由 <Repo name="@unocss/transformer-directives" /> 实现。

</v-clicks>

---

# <carbon-ibm-cloud-kubernetes-service text-md /> 开发面板

<v-clicks>

<Repo fixed right-10 top-10 class="text-sm" name="webfansplz/vite-plugin-vue-devtools" text-red-500 dark:text-red-200 />

该面板可以让你在开发过程中，了解项目的方方面面，目前仅在开发环境下有效

![devtools](/tov-template/devtools.png)

</v-clicks>

---

# <carbon-not-sent text-md />  <Badge :value="1" dark:text-white text-dark>漂亮的 404 页</Badge>

<v-clicks>

<div>

   当用户访问不存在的路由时，我们应该给用户一个好看的 `404` 页面

</div>

你可以随便访问一个不存在的页面，例如 `/bucunzai`

![notFound-dark](/tov-template/notFound-dark.png)

</v-clicks>

---

# <carbon-not-sent text-md /> <Badge :value="2" dark:text-white text-dark>漂亮的 404 页</Badge>


<v-clicks>

<div>

如果你不喜欢这个 `404` 封面，也可以在 `pages/[...notFound].vue` 中修改 `img` 标签的 `src`。

</div>

默认是 `32.svg`，支持 `1 ~ 33` 的 `svg`。

```html{|5}
<!-- 省略各种代码 -->
<template>
	<img 
      class="cover" 
      src="/notFound/32.svg" 
      alt="page not found" />
</template>
```

</v-clicks>

---
layout: center 
class: text-center 
growX: 50 
growY: 0
---

# 开源在

<Repo name="dishait/tov-template" />


---
layout: intro 
class: text-center
growX: 20 
growY: 80
---


<img src="/avatar.png" rounded-full w-35 inline-block/>

<div mb-10 mt-5>
   <Repo name="markthree" />
</div>


# Thank You!


<footer>
  ppt power by <Repo name="slidevjs/slidev"/>
</footer>