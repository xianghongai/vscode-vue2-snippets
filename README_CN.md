# Vue 2 Snippet (Visual Studio Code)

## 背景

简单的、不需要刻意记忆的代码片断，能显著提升编码效率。

一些常用的已经处理成“下意识”的触发，如我想在 `option` 中声明生命周期 (`lifecycle`) 钩子函数： `before destroy`，按 `olbd` 回车，即可生成 `beforeDestroy() {  },`；

又如，我想声明一个 `props`，是 `string` 类型的，带 `default` 属性，按 `psd` 回车，即可生成：

```js
property: {
  type: String,
  default: '',
},
```

建议大致看一下源码，去了解一下常用的 snippet 前缀。

源码目录已经做了良好的分层，方便查看对应主题的内容。

前期适应可能需要花一点点时间，慢慢的就会习惯这种快捷方式，毕竟 “There is nothing new under the coding”，形式上来来去去就那些；如果您能习惯这套方案，希望您能进行一个好的[评价](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue2-snippets&ssr=false#review-details)，并推荐给朋友，谢谢 :)

## 安装

🏳️‍🌈🏳️‍🌈🏳️‍🌈 另外还需要安装：

- [Vue Basic Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue-basic-snippets), 包含 Vue 2 和 3 中共用的 `v-*` 系列指令、`import` 组件、指令、服务之类的代码。
- [Vue 3 Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue3-snippets), 参考 Vue 3 官方文档示例及测试用例源码。
- [Pinia Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-pinia-snippets), 参考 Pinia 官方文档示例。
- [VueX Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vuex-snippets), 参考 VueX 官方文档示例、测试用例源码。
- [JavaScript Code Snippet](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-javascript-snippet), 参考 MDN 文档。
- [JavaScript Comment Snippet](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-javascript-comment), 参考 JSDOC、ESDOC 文档，用于便捷编写 JavaScript 注释。

Vue (v2.x) + Vue Router (v3.x) 代码片断

- 100% 涵盖了 vuejs.org 官方文档中的 api
- 98% 涵盖了 router.vuejs.org 官方文档中的 api

## 规划

![](https://raw.githubusercontent.com/caringrun/assets/master/vscode-vue-snippets.png)

Vue 2 和 3 Template Directives 部分一样 （vscode-vue-basic-snippets）。

Vue 2 和 3 变化比较大，2 推荐 Optional 范式，3 推荐 Composition Functions 范式。Vue 中常用的 “Global API、Directives、Transition、Async Components、Instance Events、Lifecycle” 都发生了较大的变化。并且 VueX 也推出了 4 版本。

另外随着 “reactive refs”、“Teleport” 新特性的引入，很多社区资源的升级都将是较大的变化。

因此将 Vue 2 和 3 的 Code Snippets 设计在一起，是不好的。

最好将 Vue 2 和 3 的 Code Snippets 各自分开，在项目中根据实际情况，在扩展中选择 `Disable (Workspace)`，如果觉得这样比较繁琐，可以在 “VS Code” 中安装 2 版本支持的扩展，在 “VS Code - Insiders” 中安装 3 版本支持的扩展。

---

![](https://raw.githubusercontent.com/caringrun/assets/master/vscode-vue2-snippets.gif)

## Supported languages (file extensions)

- JavaScript (`.js`)
- TypeScript (`.ts`)
- Vue (`.vue`)

## `UNSAFE` 前后缀

`UNSAFE_api/prefix`，`prefix`, 前缀风格，说明这个 API 在**当前版本**中不推荐使用；

`api/prefix_UNSAFE`，`suffix`, 后缀风格，说明这个 API 在**未来版本**中不推荐使用。


## 相关资源 🤞

- [JavaScript Code Snippet - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-javascript-snippet)
- [JavaScript Comment Snippet - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-javascript-comment)
- [React Snippets - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-react-snippet)

## Snippets

- Vue
    * Single File Component
- JavaScript/TypeScript/Vue
    * Global Config, **Vue 3 DEPRECATED!**
    * Global Data, **Vue 3 DEPRECATED!**
    * Components
    * Directives
    * Extend
    * Filters, **Vue 3 REMOVED!**
    * Mixin, **Vue 3.x BREAKING CHANGE.**
    * Plugins
    * Template
    * Instance Methods Data
    * Instance Methods Events
    * Instance Methods Lifecycle
    * Instance Properties
    * Options Composition
    * Options Data
    * Options Dom
    * Options Lifecycle Hooks
    * Options Misc
    * Options Props, Vue 3.x `Props` default value factory functions no longer have access to `this`.
- Vue Router


### Vue 🦢

单文件组件的文件名应该要么始终是单词大写开头 (PascalCase)，要么始终是横线连接 (kebab-case)。

- `vue`, 使用 SCSS 的单文件组件文件
- `vueSass`, 使用 SASS 的单文件组件文件
- `vueLess`, 使用 LESS 的单文件组件文件
- `vuePostCSS`, 使用 PostCSS 的单文件组件文件
- `vueCSS`, 使用 CSS 的单文件组件文件
- `vueStylus`, 使用 Stylus 的单文件组件文件
- `vueTypeScript`, 使用 TypeScript 的单文件组件文件
- `vueTypeScriptClass`, 使用 TypeScript（类风格） 的单文件组件文件
- `vueNoStyle`, 使用 No Style 的单文件组件文件
- `vueTemplate`, Vue `＜template＞` 元素
- `vueScript`, Vue `＜script＞` 元素
- `vueStyle`/`styleLang`, Vue `＜style＞` 元素

### JavaScript/TypeScript/Vue 🌿

#### 文件导入

- `importFilter_UNSAFE` / `ivf_UNSAFE`, `import Feature from '@/filters/Feature';` **Vue 3 REMOVED!**
- `importVueRouter`, `import VueRouter from 'vue-router';`
- `importVuex`, `import Vuex from 'vuex';`
- `importVuexHelpers`, `import { mapState, mapGetters, mapMutations, mapActions } from 'vuex';`

#### Directives

 - `Vue.directive()_UNSAFE` / `vgd_UNSAFE`, vue global directive (all hooks)
 - `Vue.directive()_UNSAFE` / `vgd_UNSAFE`, vue global directive (bind, update)
 - `Vue.directive()_UNSAFE`, retrieve global directive
 - `vueDirective` / `vsd`, vue single file directive (all hooks)
 - `option.directives` / `vld`, vue local directives
 - `directive.bind` / `vd.bind`, **v**ue **d**irective bind hook
 - `directive.inserted` / `vd.inserted`, **v**ue **d**irective inserted hook
 - `directive.update` / `vd.update`, **v**ue **d**irective update hook
 - `directive.componentUpdated` / `vd.componentUpdated`, **v**ue **d**irective componentUpdated hook
 - `directive.unbind` / `vd.unbind`, **v**ue **d**irective unbind hook

#### Options

##### Lifecycle

**O**ptions API 中的 **L**ifecycle Hooks。

- `ol`, Vue <ins>O</ins>ption <ins>L</ins>ifecycle Hooks
- `lifecycleBeforeCreate` / `option.beforeCreate()` / `olbc`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>b</ins>efore<ins>C</ins>reate()
- `lifecycleCreated` / `option.created()` / `olc`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>c</ins>reated()
- `lifecycleBeforeMount` / `option.beforeMount()` / `olbm`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>b</ins>efore<ins>M</ins>ount()
- `lifecycleMounted` / `option.mounted()` / `olm`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>m</ins>ounted()
- `lifecycleBeforeUpdate` / `option.beforeUpdate()` / `olbu`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>b</ins>efore<ins>U</ins>pdate()
- `lifecycleUpdated` / `option.updated()` / `olu`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>u</ins>pdated()
- `lifecycleActivated` / `option.activated()` / `ola`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>a</ins>ctivated()
- `lifecycleDeactivated` / `option.deactivated()` / `olda`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>d</ins>e<ins>a</ins>ctivated()
- `lifecycleBeforeDestroy` / `option.beforeDestroy()` / `olbd`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>b</ins>efore<ins>D</ins>estroy()
- `lifecycleDestroyed` / `option.destroyed()` / `old`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>d</ins>estroyed()
- `lifecycleErrorCaptured` / `option.errorCaptured()` / `olec`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>e</ins>rror<ins>C</ins>aptured()
- `lifecycleServerCacheKey` / `option.serverCacheKey()` / `olsck`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>s</ins>erver<ins>C</ins>ache<ins>K</ins>ey()
- `lifecycleServerPrefetch` / `option.serverPrefetch()` / `olsp`, <ins>o</ins>ption <ins>l</ins>ifecycle hooks: <ins>s</ins>erver<ins>P</ins>refetch()

<ins>As</ins>ync Lifecycle Hooks:

- `lifecycleAsyncCreated` / `async.option.created()` / `asolc`, <ins>As</ins>ync <ins>O</ins>ptions <ins>L</ins>ifecycle - async <ins>c</ins>reated()
- `lifecycleAsyncMounted` / `async.option.mounted()` / `asolm`, <ins>As</ins>ync <ins>O</ins>ptions <ins>L</ins>ifecycle - async <ins>m</ins>ounted()
- `lifecycleAsyncUpdated` / `async.option.updated()` / `asolu`, <ins>As</ins>ync <ins>O</ins>ptions <ins>L</ins>ifecycle - async <ins>u</ins>pdated()
- `lifecycleAsyncActivated` / `async.option.activated()` / `asola`, <ins>As</ins>ync <ins>O</ins>ptions <ins>L</ins>ifecycle - async <ins>a</ins>ctivated()
- `lifecycleAsyncDeactivated` / `async.option.deactivated()` / `asolda`, <ins>As</ins>ync <ins>O</ins>ptions <ins>L</ins>ifecycle - async <ins>de</ins>activated()

```js
  // asolc ->                            async options lifecycle created
  async created() {

  },
```


##### Option

- `option.name`- **o**ption **n**ame
- `option.functional`
- `option.delimiters`
- `option.comments`
- `option.components`, **o**ption **c**omponent**s**
- `option.directives`
- `option.filters_UNSAFE`- **Vue 3 REMOVED!**
- `option.mixins`, uses mixin
- `option.extends`
- `option.inheritAttrs`
- `option.model`
- `option.props`, **o**ption **p**rops
- `option.propsData`, option propsData
- `option.data()`, **o**ption **d**ata()
- `option.methods`, **o**ption **m**ethod**s**
- `option.provide`, **o**ption **p**rovid**e**
- `option.inject`, **o**ption **i**njec**t**
- `option.template`, **o**ption **t**emplat**e**
- `option.render`, **o**ption **r**ender
- `option.renderError`

###### Computed

- `option.computed`, <ins>o</ins>ption <ins>c</ins>ompute**d**
- `option.computedProperty`, <ins>c</ins>omputed <ins>p</ins>roperty

```js
  // ocd ->                            // options computed
  computed: {
    property() {
      return this.property;
    },

    // cp ->                            // computed property
    property() {
      return this.property;
    },

  },
```

###### Watch

- `option.watch`, **o**ption **w**atch
- `option.watchProperty`, **o**ption **w**atch **p**roperty
- `option.watchPropertyDeep`, **o**ption **w**atch **p**roperty (**d**eep)
- `option.watchPropertyImmediate`, **o**ption **w**atch **p**roperty (**i**mmediate)
- `option.watchPropertyDeepImmediate`, **o**ption **w**atch **p**roperty (**d**eep, **i**mmediate)

```js
  // ow ->                            // options watch
  watch: {
    propertyName(newValue, oldValue) {

    },

    // wpdi ->                            // watch property (deep, immediate)
    propertyName: {
      deep: true,
      immediate: true,
      handler(newValue, oldValue) {

      },
    },
  },
```

##### Composition/DOM/Misc

- `el`
- `template`
- `render(h, context)`
- `renderError(h, err)`

#### Props

- `propOptions`, **o**ptions **p**rop, 输入 `op` 试试
- `propString`, **p**rop **s**tring, 输入 `ps` 试试
- `propNumber`, **p**rop **n**umber
- `propBoolean`, **p**rop **b**oolean
- `propArray`, **p**rop **a**rray
- `propObject`, **p**rop **o**bject
- `propDate`, **p**rop **d**ate
- `propFunction`, **p**rop **f**unction
- `propSymbol`, **p**rop **s**ymbol
- `propPromise`, **p**rop **p**romise
- `propStringDefault`, **p**rop **s**tring (**d**efault)
- `propNumberDefault`, **p**rop **n**umber (**d**efault)
- `propBooleanDefault`, **p**rop **b**oolean (**d**efault)
- `propArrayDefault`, **p**rop **a**rray (**d**efault)
- `propObjectDefault`, **p**rop **o**bject (**d**efault)
- `propDateDefault`, **p**rop **d**ate (**d**efault)
- `propSymbolDefault`, **p**rop **s**ymbol (**d**efault)
- `propFunctionDefault`, **p**rop **f**unction (**d**efault)
- `propPromiseDefault`, **p**rop **p**romise (**d**efault)
- `propStringRequired`, **p**rop **s**tring (**r**equired)
- `propNumberRequired`, **p**rop **n**umber (**r**equired)
- `propBooleanRequired`, **p**rop **b**oolean (**r**equired)
- `propArrayRequired`, **p**rop **a**rray (**r**equired)
- `propObjectRequired`, **p**rop **o**bject (**r**equired)
- `propDateRequired`, **p**rop **d**ate (**r**equired)
- `propFunctionRequired`, **p**rop **f**unction (**r**equired)
- `propSymbolRequired`, **p**rop **s**ymbol (**r**equired)
- `propPromiseRequired`, **p**rop **p**romise (**r**equired)
- `propStringDefaultRequired`, **p**rop **s**tring (**d**efault, **r**equired)
- `propNumberDefaultRequired`, **p**rop **n**umber (**d**efault, **r**equired)
- `propBooleanDefaultRequired`, **p**rop **b**oolean (**d**efault, **r**equired)
- `propArrayDefaultRequired`, **p**rop **a**rray (**d**efault, **r**equired)
- `propObjectDefaultRequired`, **p**rop **o**bject (**d**efault, **r**equired)
- `propDateDefaultRequired`, **p**rop **d**ate (**d**efault, **r**equired)
- `propFunctionDefaultRequired`, **p**rop **f**unction (**d**efault, **r**equired)
- `propSymbolDefaultRequired`, **p**rop **s**ymbol (**d**efault, **r**equired)
- `propPromiseDefaultRequired`, **p**rop **p**romise (**d**efault, **r**equired)

#### Instance

##### Instance Properties

- `this.$data`
- `this.$props`
- `this.$el`
- `this.$options`
- `this.$parent`
- `this.$root`
- `this.$children_UNSAFE`, **Vue 3 REMOVED!**
- `this.$slots`
- `this.$scopedSlots_UNSAFE`, **Vue 3 REMOVED!**
- `this.$refs`
- `this.$isServer`
- `this.$attrs`
- `this.$listeners_UNSAFE`, **Vue 3 REMOVED!**

##### Instance Methods Lifecycle

- `this.$nextTick()`, **n**ext**T**ick
- `await this.$nextTick()`, **a**wait **n**ext**T**ick
- `this.$forceUpdate()`
- `this.$destroy()`
- `this.$mount()`


#### Instance Methods Data

- `this.$watch()`
- `this.$watch(data, cb, {deep, immediate})`
- `this.$set()`/`set`
- `this.$delete()`


#### Instance Methods Events

- `this.$on()_UNSAFE`, **Vue 3 REMOVED!**
- `this.$emit()`/`emit`
- `this.$once()_UNSAFE`, **Vue 3 REMOVED!**
- `this.$off()_UNSAFE`/`off`, **Vue 3 REMOVED!**


#### Template/Plugins/Mixin/Extend

- `Vue.compile(template)_UNSAFE`, **Vue 3.x BREAKING CHANGE.**
- `Vue.use(plugin)_UNSAFE`, **Vue 3.x BREAKING CHANGE.**
- `pluginComponent`, Create Plugin
- `pluginComponents`, Create Plugin
- `vueMixin`, Define a mixin object
- `Vue.mixin(mixin)_UNSAFE`, Global Mixin, **Vue 3.x BREAKING CHANGE.**
- `Vue.extend(options)_UNSAFE`
- `Vue.prototype_UNSAFE`, Vue Plugin add an instance method, **Vue 3.x BREAKING CHANGE.**


#### Components

- `vueGlobalComponent`/`vgc`, Vue Global Component, **Vue 3 DEPRECATED!**
- `vueFunctionalComponents`/`vfc`, Vue Functional Component, **Vue 3.x BREAKING CHANGE!**
- `vueAsyncComponents`/`vac`, `const Feature = () => import('@/views/FeaturePage.vue');`, Vue Async Components, **Vue 3.x BREAKING CHANGE!**
- `Vue.component()_UNSAFE`, Retrieve Global Component, **Vue 3 DEPRECATED!**


#### Global

**DEPRECATED!**

查看“从 Vue 2 迁移”[全局 API](https://v3.cn.vuejs.org/guide/migration/global-api.html) 和 [全局 API Treeshaking](https://v3.cn.vuejs.org/guide/migration/global-api-treeshaking.html#_2-x-%E8%AF%AD%E6%B3%95)；

##### Global Config

- `Vue.config.silent_UNSAFE`
- `Vue.config.optionMergeStrategies_UNSAFE`
- `Vue.config.devtools_UNSAFE`
- `Vue.config.errorHandler_UNSAFE`
- `Vue.config.warnHandler_UNSAFE`
- `Vue.config.ignoredElements_UNSAFE`
- `Vue.config.keyCodes_UNSAFE`
- `Vue.config.performance_UNSAFE`
- `Vue.config.productionTip_UNSAFE`

##### Global Data

- `Vue.nextTick([callback, context])_UNSAFE`
- `Vue.nextTick().then()_UNSAFE`
- `Vue.set(target, propertyName/index, value)_UNSAFE`
- `Vue.delete(target, propertyName/index)_UNSAFE`
- `Vue.observable(object)_UNSAFE`


#### Vue Router

- `router` / `newVueRouter`, Create the router instance
- `newVueRouter`, Create the router instance (import)
- `routerHistoryMode`, Create the router instance with HTML5 History Mode
- `routes`, Define routes
- `route`, Define route
- `routeLazy`, Define lazy loading route
- `routePropsBooleanMode`, Define route and pass props to route components (Boolean mode)
- `routePropsObjectMode`, Define route and pass props to route components (Object mode)
- `routePropsFunctionMode`, Define route and pass props to route components (Function mode)
- `routePropsFunctionModeNamedViews`, Define route and pass props for routes with named views (Function mode)
- `routeNamedViews`, Define route for named views
- `routeAlias`, Define alias route
- `routeRedirect`, Define redirect route
- `routeRedirectNamedRoute`, Define redirect named route
- `routeRedirectDynamic`, Define dynamic redirect
- `routeNamed`, Define named route
- `routerPush`, Router navigate to path with literal string
- `routerPushPath`, Router navigate to path
- `routerPushParams`, Router navigate to path with params
- `routerPushQuery`, Router navigate to path with query
- `routerPushNamedRoute`, Router navigate to named routes
- `routerPushNamedRouteParams`, Router navigate to named routes with params
- `routerPushNamedRouteQuery`, Router navigate to named routes with query
- `routerReplacePath`, Router navigate to path without pushing a new history entry
- `routerReplaceNamedRoute`, Router navigate to named routes without pushing a new history entry
- `routerGo`, Programmatically navigate to a new URL: go(n)
- `routerBack`, Programmatically navigate to a new URL: back()
- `routerForward`, Programmatically navigate to a new URL: forward()
- `routerResolve`, Reverse URL resolving
- `routerBeforeEach` / `guardGlobalBefore`, Global Before Guards
- `routerBeforeResolve` / `guardGlobalResolve`, Global Resolve Guards
- `routerAfterEach`, Global After Hooks
- `routeBeforeEnter` / `guardPerRoute`, Per-Route Guard
- `componentGuards` / `guardInComponent`, In-Component Guards
- `routerAddRoutes`, Dynamically add more routes to the router
- `routerOnReady`, Router instance method: onReady(callback, errorCallback)
- `routerOnError`, Router instance method: onError(callback)
- `routerGetMatchedComponents`, Router instance method: getMatchedComponents(to)
- `this.$route.path`, $route.path
- `this.$route.params`, $route.params
- `this.$route.query`, $route.query
- `this.$route.hash`, $route.hash
- `this.$route.fullPath`, $route.fullPath
- `this.$route.matched`, $route.matched
- `this.$route.name`, $route.name
- `this.$route.redirectedFrom`, $route.redirectedFrom
- `lazyRoute`, Lazy Loading Routes
- `lazyRouteChunk`, Lazy Loading Routes, Grouping Components in the Same Chunk
- `fetchingAfterNavigation`, Fetching After Navigation
- `fetchingBeforeNavigation`, Fetching Before Navigation
- `routeTransition`, Route-Based Dynamic Transition
- `vScrollbehavior`, Vue Router scrollBehavior

---

## File Name

查看“风格指南” [优先级 B 的规则：强烈推荐 (增强代码可读性)](https://v3.cn.vuejs.org/style-guide/#%E4%BC%98%E5%85%88%E7%BA%A7-b-%E7%9A%84%E8%A7%84%E5%88%99-%E5%BC%BA%E7%83%88%E6%8E%A8%E8%8D%90-%E5%A2%9E%E5%BC%BA%E4%BB%A3%E7%A0%81%E5%8F%AF%E8%AF%BB%E6%80%A7)。

## License 📃

MIT License

**Donate**

![xianghongai@gmail.com](https://raw.githubusercontent.com/caringrun/assets/master/donate.png)