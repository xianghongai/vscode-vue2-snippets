# Vue 2 Snippet (Visual Studio Code)

🏳️‍🌈🏳️‍🌈🏳️‍🌈 首先需要安装 "[Vue Basic Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue-basic-snippets)".

Vue (v2.x) + Vue Router (v3.x) + VueX (v3.x) 代码片断

- 100% 涵盖了 vuejs.org 官方文档中的 api
- 98% 涵盖了 router.vuejs.org 官方文档中的 api
- 100% 涵盖了 vuex.vuejs.org 官方文档中的 api

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

`UNSAFE_api`，`prefix`, 前缀风格，说明这个 API 在**当前版本**中不推荐使用；

`api_UNSAFE`，`suffix`, 后缀风格，说明这个 API 在**未来版本**中不推荐使用。


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
    * Vue Router
    * VueX


### Vue 🦢

单文件组件的文件名应该要么始终是单词大写开头 (PascalCase)，要么始终是横线连接 (kebab-case)。

- `vue` - 使用 SCSS 的单文件组件文件
- `vueSass` - 使用 SASS 的单文件组件文件
- `vueLess` - 使用 LESS 的单文件组件文件
- `vuePostCSS` - 使用 PostCSS 的单文件组件文件
- `vueCSS` - 使用 CSS 的单文件组件文件
- `vueStylus` - 使用 Stylus 的单文件组件文件
- `vueTypeScript` - 使用 TypeScript 的单文件组件文件
- `vueTypeScriptClass` - 使用 TypeScript（类风格） 的单文件组件文件
- `vueNoStyle` - 使用 No Style 的单文件组件文件
- `vueTemplate` - Vue `＜template＞` 元素
- `vueScript` - Vue `＜script＞` 元素
- `vueStyle`/`styleLang` - Vue `＜style＞` 元素

### JavaScript/TypeScript/Vue 🌿

#### 文件导入

- `importComponent` / `ivc` - `import Feature from '@/components/Feature';`
- `importDirective` / `ivd` - `import Feature from '@/directives/Feature';`
- `importFilter_UNSAFE` / `ivf_UNSAFE` - `import Feature from '@/filters/Feature';` **Vue 3 REMOVED!**
- `importVueRouter` - `import VueRouter from 'vue-router';`
- `importVuex` - `import Vuex from 'vuex';`
- `importVuexHelpers` - `import { mapState, mapGetters, mapMutations, mapActions } from 'vuex';`

#### Vue Router

- `router` / `newVueRouter` - Create the router instance
- `newVueRouter` - Create the router instance (import)
- `routerHistoryMode` - Create the router instance with HTML5 History Mode
- `routes` - Define routes
- `route` - Define route
- `routeLazy` - Define lazy loading route
- `routePropsBooleanMode` - Define route and pass props to route components (Boolean mode)
- `routePropsObjectMode` - Define route and pass props to route components (Object mode)
- `routePropsFunctionMode` - Define route and pass props to route components (Function mode)
- `routePropsFunctionModeNamedViews` - Define route and pass props for routes with named views (Function mode)
- `routeNamedViews` - Define route for named views
- `routeAlias` - Define alias route
- `routeRedirect` - Define redirect route
- `routeRedirectNamedRoute` - Define redirect named route
- `routeRedirectDynamic` - Define dynamic redirect
- `routeNamed` - Define named route
- `routerPush` - Router navigate to path with literal string
- `routerPushPath` - Router navigate to path
- `routerPushParams` - Router navigate to path with params
- `routerPushQuery` - Router navigate to path with query
- `routerPushNamedRoute` - Router navigate to named routes
- `routerPushNamedRouteParams` - Router navigate to named routes with params
- `routerPushNamedRouteQuery` - Router navigate to named routes with query
- `routerReplacePath` - Router navigate to path without pushing a new history entry
- `routerReplaceNamedRoute` - Router navigate to named routes without pushing a new history entry
- `routerGo` - Programmatically navigate to a new URL: go(n)
- `routerBack` - Programmatically navigate to a new URL: back()
- `routerForward` - Programmatically navigate to a new URL: forward()
- `routerResolve` - Reverse URL resolving
- `routerBeforeEach` / `guardGlobalBefore` - Global Before Guards
- `routerBeforeResolve` / `guardGlobalResolve` - Global Resolve Guards
- `routerAfterEach` - Global After Hooks
- `routeBeforeEnter` / `guardPerRoute` - Per-Route Guard
- `componentGuards` / `guardInComponent` - In-Component Guards
- `routerAddRoutes` - Dynamically add more routes to the router
- `routerOnReady` - Router instance method: onReady(callback, errorCallback)
- `routerOnError` - Router instance method: onError(callback)
- `routerGetMatchedComponents` - Router instance method: getMatchedComponents(to)
- `this.$route.path` - $route.path
- `this.$route.params` - $route.params
- `this.$route.query` - $route.query
- `this.$route.hash` - $route.hash
- `this.$route.fullPath` - $route.fullPath
- `this.$route.matched` - $route.matched
- `this.$route.name` - $route.name
- `this.$route.redirectedFrom` - $route.redirectedFrom
- `lazyRoute` - Lazy Loading Routes
- `lazyRouteChunk` - Lazy Loading Routes, Grouping Components in the Same Chunk
- `fetchingAfterNavigation` - Fetching After Navigation
- `fetchingBeforeNavigation` - Fetching Before Navigation
- `routeTransition` - Route-Based Dynamic Transition
- `vScrollbehavior` - Vue Router scrollBehavior

#### VueX

- `newVuex` - Create the Vuex instance
- `vuexGetters` - Vuex Getters
- `vuexModules` - Vuex Modules
- `action` - Actions property
- `action` - Actions property (Promise)
- `action` - Actions property (Async/Await)
- `mapState` - mapState (array)
- `mapState` - mapState (object)
- `mapGetters` - mapGetters (array)
- `mapGetters` - mapGetters (object)
- `mapMutations` - mapMutations (array)
- `mapMutations` - mapMutations (object)
- `mapActions` - mapActions (array)
- `mapActions` - mapActions (object)
- `createNamespacedHelpers` - createNamespacedHelpers
- `store.getters` - store.getters
- `store.state` - store.state
- `store.commit()` / `sc` - store.commit(type, payload, options)
- `store.dispatch()` / `sd` - store.dispatch(type, payload)
- `store.dispatch()` / `sdp` - store.dispatch(type, payload), promise
- `store.replaceState()` - store.replaceState(state)
- `store.watch()` - store.watch(getter, cb, options)
- `store.subscribe()` - store.subscribe(fn, options)
- `store.subscribeAction()` - store.subscribeAction(fn, options)
- `store.subscribeAction()` - store.subscribeAction(object)
- `store.registerModule()` - store.registerModule(path, rawModule, options)
- `store.unregisterModule()` - store.unregisterModule(path)
- `store.hasModule()` - store.hasModule(path)
- `store.hotUpdate()` - store.hotUpdate(newOptions)


#### Directives

 - `Vue.directive()_UNSAFE` / `vgd_UNSAFE` - Vue Global Directive (All Hooks)
 - `Vue.directive()_UNSAFE` / `vgd_UNSAFE` - Vue Global Directive (bind, update)
 - `Vue.directive()_UNSAFE` - Retrieve Global Directive
 - `vueDirective` / `vsd` - Vue Single File Directive (All Hooks)
 - `option.directives` / `vld` - Vue Local Directives
 - `directive.bind` / `vd.bind` - **V**ue **D**irective bind hook
 - `directive.inserted` / `vd.inserted` - **V**ue **D**irective inserted hook
 - `directive.update` / `vd.update` - **V**ue **D**irective update hook
 - `directive.componentUpdated` / `vd.componentUpdated` - **V**ue **D**irective componentUpdated hook
 - `directive.unbind` / `vd.unbind` - **V**ue **D**irective unbind hook


#### Options

##### Lifecycle

- `vlh` - The **V**ue Instance Full **L**ifecycle **H**ooks
- `lifecycleBeforeCreate` / `option.beforeCreate()` / `vlh.beforeCreate()` - **V**ue instance **L**ifecycle **H**ooks: beforeCreate()
- `lifecycleCreated` / `option.created()` / `vlh.created()` - **V**ue instance **L**ifecycle **H**ooks: created()
- `lifecycleBeforeMount` / `option.beforeMount()` / `vlh.beforeMount()` - **V**ue instance **L**ifecycle **H**ooks: beforeMount()
- `lifecycleMounted` / `option.mounted()` / `vlh.mounted()` - **V**ue instance **L**ifecycle **H**ooks: mounted()
- `lifecycleBeforeUpdate` / `option.beforeUpdate()` / `vlh.beforeUpdate()` - **V**ue instance **L**ifecycle **H**ooks: beforeUpdate()
- `lifecycleUpdated` / `option.updated()` / `vlh.updated()` - **V**ue instance **L**ifecycle **H**ooks: updated()
- `lifecycleActivated` / `option.activated()` / `vlh.activated()` - **V**ue instance **L**ifecycle **H**ooks: activated()
- `lifecycleDeactivated` / `option.deactivated()` / `vlh.deactivated()` - **V**ue instance **L**ifecycle **H**ooks: deactivated()
- `lifecycleBeforeDestroy` / `option.beforeDestroy()` / `vlh.beforeDestroy()` - **V**ue instance **L**ifecycle **H**ooks: beforeDestroy()
- `lifecycleDestroyed` / `option.destroyed()` / `vlh.destroyed()` - **V**ue instance **L**ifecycle **H**ooks: destroyed()
- `lifecycleErrorCaptured` / `option.errorCaptured()` / `vlh.errorCaptured()` - **V**ue instance **L**ifecycle **H**ooks: errorCaptured()
- `lifecycleServerCacheKey` / `option.serverCacheKey()` / `vlh.serverCacheKey()` - **V**ue instance **L**ifecycle **H**ooks: serverCacheKey()
- `lifecycleServerPrefetch` / `option.serverPrefetch()` / `vlh.serverPrefetch()` - **V**ue instance **L**ifecycle **H**ooks: serverPrefetch()

##### Option

- `option.name`
- `option.functional`
- `option.delimiters`
- `option.comments`
- `option.components`
- `option.directives`
- `option.filters_UNSAFE`, **Vue 3 REMOVED!**
- `option.mixins` - uses mixin
- `option.extends`
- `option.inheritAttrs`
- `option.model`
- `option.props` - option props
- `option.propsData` - option propsData
- `option.data()` - option data()
- `option.computed` - option computed
- `option.watch` - option watch
- `option.watchProperty` - option watch property
- `option.watchPropertyDeep` - option watch property (deep)
- `option.watchPropertyImmediate` - option watch property (immediate)
- `option.watchPropertyDeepImmediate` - option watch property (deep, immediate)
- `option.methods` - option methods
- `option.provide`
- `option.inject`
- `option.template`
- `option.render`
- `option.renderError`

##### Composition/DOM/Misc

- `el`
- `template`
- `render(h, context)`
- `renderError(h, err)`


#### Props

- `propOptions` - Prop Options
- `propString` - String
- `propNumber` - Number
- `propBoolean` - Boolean
- `propArray` - Array
- `propObject` - Object
- `propDate` - Date
- `propFunction` - Function
- `propSymbol` - Symbol
- `propPromise` - Promise
- `propStringDefault` - String (default)
- `propNumberDefault` - Number (default)
- `propBooleanDefault` - Boolean (default)
- `propArrayDefault` - Array (default)
- `propObjectDefault` - Object (default)
- `propDateDefault` - Date (default)
- `propSymbolDefault` - Symbol (default)
- `propFunctionDefault` - Function (default)
- `propPromiseDefault` - Promise (default)
- `propStringRequired` - String (required)
- `propNumberRequired` - Number (required)
- `propBooleanRequired` - Boolean (required)
- `propArrayRequired` - Array (required)
- `propObjectRequired` - Object (required)
- `propDateRequired` - Date (required)
- `propFunctionRequired` - Function (required)
- `propSymbolRequired` - Symbol (required)
- `propPromiseRequired` - Promise (required)
- `propStringDefaultRequired` - String (default, required)
- `propNumberDefaultRequired` - Number (default, required)
- `propBooleanDefaultRequired` - Boolean (default, required)
- `propArrayDefaultRequired` - Array (default, required)
- `propObjectDefaultRequired` - Object (default, required)
- `propDateDefaultRequired` - Date (default, required)
- `propFunctionDefaultRequired` - Function (default, required)
- `propSymbolDefaultRequired` - Symbol (default, required)
- `propPromiseDefaultRequired` - Promise (default, required)

尝试一下 `pPDR`，其它部分可以同样操作。

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

- `this.$nextTick()`
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
- `pluginComponent` - Create Plugin
- `pluginComponents` - Create Plugin
- `vueMixin` - Define a mixin object
- `Vue.mixin(mixin)_UNSAFE` - Global Mixin, **Vue 3.x BREAKING CHANGE.**
- `Vue.extend(options)_UNSAFE`
- `Vue.prototype_UNSAFE` - Vue Plugin add an instance method, **Vue 3.x BREAKING CHANGE.**


#### Components

- `vueGlobalComponent`/`vgc` - Vue Global Component, **Vue 3 DEPRECATED!**
- `vueFunctionalComponents`/`vfc` - Vue Functional Component, **Vue 3.x BREAKING CHANGE!**
- `vueAsyncComponents`/`vac` - `const Feature = () => import('@/views/FeaturePage.vue');` - Vue Async Components, **Vue 3.x BREAKING CHANGE!**
- `Vue.component()_UNSAFE` - Retrieve Global Component, **Vue 3 DEPRECATED!**


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


---

## File Name

查看“风格指南” [优先级 B 的规则：强烈推荐 (增强代码可读性)](https://v3.cn.vuejs.org/style-guide/#%E4%BC%98%E5%85%88%E7%BA%A7-b-%E7%9A%84%E8%A7%84%E5%88%99-%E5%BC%BA%E7%83%88%E6%8E%A8%E8%8D%90-%E5%A2%9E%E5%BC%BA%E4%BB%A3%E7%A0%81%E5%8F%AF%E8%AF%BB%E6%80%A7)。

- foo-bar`${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/g}`, .vue  →  `name: FooBar`;
- foo-bar`${TM_FILENAME_BASE}`, .vue  →  `name: foo-bar`;
- foo-bar`${TM_DIRECTORY}`, /index.vue  →  `name: foo-bar`;


## License 📃

MIT License

---

TODO: vue-ssr


**Donate**

![xianghongai@gmail.com](https://raw.githubusercontent.com/caringrun/assets/master/donate.png)