<p>
  <h1 align="center">Vue 2 Snippet (Visual Studio Code)</h1>
</p>

<p align="center">
  <a href="https://github.com/xianghongai/vscode-vue2-snippets">
    <img src="https://img.shields.io/github/repo-size/xianghongai/vscode-vue2-snippets?style=plastic&color=4ac51c">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue2-snippets">
    <img src="https://vsmarketplacebadge.apphb.com/version-short/NicholasHsiang.vscode-vue2-snippets.svg?style=plastic&color=42a5f5">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue2-snippets">
    <img src="https://vsmarketplacebadge.apphb.com/installs-short/NicholasHsiang.vscode-vue2-snippets.svg?style=plastic&color=4ac51c">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue2-snippets">
    <img src="https://vsmarketplacebadge.apphb.com/rating-short/NicholasHsiang.vscode-vue2-snippets.svg?style=plastic&color=4ac51c">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue2-snippets">
    <img src="https://img.shields.io/github/license/xianghongai/vscode-vue2-snippets?maxAge=2592000&style=plastic&color=4ac51c">
  </a>
</p>

[中文](./README_CN.md)

## Beginning

Simple code snippets that don’t need to be memorized, It can significantly improve coding efficiency.

Some commonly used triggers that have been processed as "subconscious", such as I want to declare the **o**ption **l**ifecycle hook function **b**efore **d**estroy: , press `olbd` and press Enter to output `beforeDestroy() {},`;

For another example, I want to create a `props`, which is of type `string`, with a `default` property, and press `psd` to output:

```js
property: {
  type: String,
  default: '',
},
```

It is recommended to take a look at the source code to learn about common snippet prefixes.

The source code directory has been well layered, It is convenient to view the content of the corresponding topic.

It may take a little time to adapt in the early stage, and you will gradually get used to this shortcut.

## Install

🌈🌈🌈 **First need to install "[Vue Basic Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue-basic-snippets)"** (template directive), they are one combined release.

Code snippets for Vue (v2.x) + Vue Router (v3.x) + VueX (v3.x).

- 100% covered vuejs.org official document api
- 98% covered router.vuejs.org official document api
- 100% covered vuex.vuejs.org official document api

## Design

![](https://raw.githubusercontent.com/caringrun/assets/master/vscode-vue-snippets.png)

Vue 2 and 3 Template Directives are the same (vscode-vue-basic-snippets).

Vue 2 and 3 have relatively large changes, 2 recommends the Optional paradigm, and 3 recommends the Composition Functions paradigm. The commonly used "Global API, Directives, Transition, Async Components, Instance Events, Lifecycle" in Vue have undergone major changes. And VueX also launched 4 versions.

In addition, with the introduction of new features of "reactive refs" and "Teleport", the upgrade of many community resources will be major changes.

Therefore, it is not good to design Vue 2 and 3 Code Snippets together.

It is best to separate the Code Snippets of Vue 2 and 3 respectively. According to the actual situation in the project, select `Disable (Workspace)` in the extension. If you feel this is more cumbersome, you can install the extension supported by version 2 in "`VS Code`" , Install the extensions supported by version 3 in "`VS Code-Insiders`".

---

![](https://raw.githubusercontent.com/caringrun/assets/master/vscode-vue2-snippets.gif)

## Supported languages (file extensions)

- JavaScript (`.js`)
- TypeScript (`.ts`)
- HTML (`.html`)
- Vue (`.vue`)

## The `UNSAFE` prefix/suffix

`UNSAFE_api`，`prefix`, Indicates that it is deprecated in the **current** version.

`api_UNSAFE`，`suffix`, Indicates that it has been deprecated in **future** versions.


## Resources 🤞

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

- `vue`, Vue Single File Component with SCSS
- `vueSass`, Vue Single File Component with SASS
- `vueLess`, Vue Single File Component with LESS
- `vuePostCSS`, Vue Single File Component with PostCSS
- `vueCSS`, Vue Single File Component with CSS
- `vueStylus`, Vue Single File Component with Stylus
- `vueTypeScript`, Vue Single File Component with TypeScript
- `vueTypeScriptClass`, Vue Single File Component with Class based TypeScript format
- `vueNoStyle`, Vue Single File Component with No Style
- `vueTemplate`, Vue Template element
- `vueScript`, Vue Script element
- `vueStyle`/`styleLang`, Vue Style element

### JavaScript/TypeScript/Vue 🌿

#### Import/Instance

- `importFilter_UNSAFE` / `ivf_UNSAFE`, `import Feature from '@/filters/Feature';` **Vue 3 REMOVED!**
- `importVueRouter`, `import VueRouter from 'vue-router';`
- `importVuex`, `import Vuex from 'vuex';`
- `importVuexHelpers`, `import { mapState, mapGetters, mapMutations, mapActions } from 'vuex';`
- `newVue`, Vue Instance

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

#### VueX

- `newVuex`, Create the Vuex instance
- `vuexGetters`, Vuex Getters
- `vuexModules`, Vuex Modules
- `action`, Actions property
- `action`, Actions property (Promise)
- `action`, Actions property (Async/Await)
- `mapState`, mapState (array)
- `mapState`, mapState (object)
- `mapGetters`, mapGetters (array)
- `mapGetters`, mapGetters (object)
- `mapMutations`, mapMutations (array)
- `mapMutations`, mapMutations (object)
- `mapActions`, mapActions (array)
- `mapActions`, mapActions (object)
- `createNamespacedHelpers`, createNamespacedHelpers
- `store.getters`, [this.]store.getters
- `store.state`, [this.]store.state
- `store.commit()` / `sc`, [this.]store.commit(type, payload, options)
- `store.dispatch()` / `sd`, [this.]store.dispatch(type, payload)
- `store.dispatch()` / `sdp`, [this.]store.dispatch(type, payload), promise
- `store.replaceState()`, [this.]store.replaceState(state)
- `store.watch()`, [this.]store.watch(getter, cb, options)
- `store.subscribe()`, [this.]store.subscribe(fn, options)
- `store.subscribeAction()`, [this.]store.subscribeAction(fn, options)
- `store.subscribeAction()`, [this.]store.subscribeAction(object)
- `store.registerModule()`, [this.]store.registerModule(path, rawModule, options)
- `store.unregisterModule()`, [this.]store.unregisterModule(path)
- `store.hasModule()`, [this.]store.hasModule(path)
- `store.hotUpdate()`, [this.]store.hotUpdate(newOptions)


#### Directives

 - `Vue.directive()_UNSAFE` / `vgd_UNSAFE`, vue global directive (all hooks)
 - `Vue.directive()_UNSAFE` / `vgd_UNSAFE`, vue global directive (bind, update)
 - `Vue.directive()_UNSAFE`, retrieve global directive
 - `vueDirective` / `vsd`, vue single file directive (all hooks)
 - `option.directives` / `vld`, **v**ue **l**ocal **d**irectives
 - `directive.bind` / `vd.bind`, **v**ue **d**irective bind hook
 - `directive.inserted` / `vd.inserted`, **v**ue **d**irective inserted hook
 - `directive.update` / `vd.update`, **v**ue **d**irective update hook
 - `directive.componentUpdated` / `vd.componentUpdated`, **v**ue **d**irective componentUpdated hook
 - `directive.unbind` / `vd.unbind`, **v**ue **d**irective unbind hook


#### Options

##### Lifecycle

- `ol`, Vue **O**ption **L**ifecycle Hooks
- `lifecycleBeforeCreate` / `option.beforeCreate()` / `olbc`, vue **o**ption **l**ifecycle hooks: **b**efore**C**reate()
- `lifecycleCreated` / `option.created()` / `olc`, vue **o**ption **l**ifecycle hooks: **c**reated()
- `lifecycleCreatedAsync` / `async.option.created()` / `aolc`, **A**sync vue **o**ption **l**ifecycle hooks: **c**reated()
- `lifecycleBeforeMount` / `option.beforeMount()` / `olbm`, vue **o**ption **l**ifecycle hooks: **b**efore**M**ount()
- `lifecycleMounted` / `option.mounted()` / `olm`, vue **o**ption **l**ifecycle hooks: **m**ounted()
- `lifecycleMountedAsync` / `async.option.mounted()` / `aolm`, **A**sync vue **o**ption **l**ifecycle hooks: **m**ounted()
- `lifecycleBeforeUpdate` / `option.beforeUpdate()` / `olbu`, vue **o**ption **l**ifecycle hooks: **b**efore**U**pdate()
- `lifecycleUpdated` / `option.updated()` / `olu`, vue **o**ption **l**ifecycle hooks: **u**pdated()
- `lifecycleActivated` / `option.activated()` / `ola`, vue **o**ption **l**ifecycle hooks: **a**ctivated()
- `lifecycleDeactivated` / `option.deactivated()` / `olda`, vue **o**ption **l**ifecycle hooks: **d**e**a**ctivated()
- `lifecycleBeforeDestroy` / `option.beforeDestroy()` / `olbd`, vue **o**ption **l**ifecycle hooks: **b**efore**D**estroy()
- `lifecycleDestroyed` / `option.destroyed()` / `old`, vue **o**ption **l**ifecycle hooks: **d**estroyed()
- `lifecycleErrorCaptured` / `option.errorCaptured()` / `olec`, vue **o**ption **l**ifecycle hooks: **e**rror**C**aptured()
- `lifecycleServerCacheKey` / `option.serverCacheKey()` / `olsck`, vue **o**ption **l**ifecycle hooks: **s**erver**C**ache**K**ey()
- `lifecycleServerPrefetch` / `option.serverPrefetch()` / `olsp`, vue **o**ption **l**ifecycle hooks: **s**erver**P**refetch()

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
- `option.computed`, **o**ption **c**ompute**d**
- `option.watch`, **o**ption **w**atch
- `option.watchProperty`, **o**ption **w**atch **p**roperty
- `option.watchPropertyDeep`, **o**ption **w**atch **p**roperty (**d**eep)
- `option.watchPropertyImmediate`, **o**ption **w**atch **p**roperty (**i**mmediate)
- `option.watchPropertyDeepImmediate`, **o**ption **w**atch **p**roperty (**d**eep, **i**mmediate)
- `option.methods`, **o**ption **m**ethod**s**
- `option.provide`, **o**ption **p**rovid**e**
- `option.inject`, **o**ption **i**njec**t**
- `option.template`, **o**ption **t**emplat**e**
- `option.render`, **o**ption **r**ender
- `option.renderError`

##### Composition/DOM/Misc

- `el`
- `template`
- `render(h, context)`
- `renderError(h, err)`


#### Props

- `propOptions`, **o**ptions **p**rop
- `propString`, **p**rop **s**tring
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

View "Migration from Vue 2" [Global API](https://v3.vuejs.org/guide/migration/global-api.html), [Global API Treeshaking](https://v3.vuejs.org/guide/migration/global-api-treeshaking.html).

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

View "Style Guide" [Priority B Rules: Strongly Recommended (Improving Readability)](https://v3.vuejs.org/style-guide/#priority-b-rules-strongly-recommended-improving-readability).

## License 📃

MIT License

---

**Donate**

![xianghongai@gmail.com](https://raw.githubusercontent.com/caringrun/assets/master/donate.png)
