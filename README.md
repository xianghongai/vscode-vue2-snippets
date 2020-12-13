# Vue2 Snippet (Visual Studio Code)

Code snippets for Vue (v2.x) + Vue Router (v3.x) + VueX (v3.x).  [中文](./README_CN.md)

- 100% covered vuejs.org official document api
- 98% covered router.vuejs.org official document api
- 100% covered vuex.vuejs.org official document api

## Design

Vue 2 and 3 have relatively large changes, 2 recommends the Optional paradigm, and 3 recommends the Composition Functions paradigm. The commonly used "Global API, Directives, Transition, Async Components, Instance Events, Lifecycle" in Vue have undergone major changes. And VueX also launched 4 versions.

In addition, with the introduction of new features of "reactive refs" and "Teleport", the upgrade of many community resources will be major changes.

Therefore, it is not good to design Vue 2 and 3 Code Snippets together.

It is best to separate the Code Snippets of Vue 2 and 3 respectively. According to the actual situation in the project, select `Disable (Workspace)` in the extension. If you feel this is more cumbersome, you can install the extension supported by version 2 in "`VS Code`" , Install the extensions supported by version 3 in "`VS Code-Insiders`".

---

![](https://raw.githubusercontent.com/caringrun/assets/master/vscode-vue2-snippets.gif)

## Supported languages (file extensions)

- JavaScript (`.js`)
- TypeScript (`.ts`)
- Html (`.html`)
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
    * Transition
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
- HTML
    * Built In Components
        + Dynamic Component
        + Keep Alive
        + Slot
        + Transition
    * Directives
    * Instance Methods Events
    * Refs, Key
    * Style & Class
    * Vue Router
    * Transition
- Style
    * v-cloak
    * Transition


### Vue 🦢

- `vue` - Vue Single File Component with SCSS
- `vueSass` - Vue Single File Component with SASS
- `vueLess` - Vue Single File Component with LESS
- `vuePostCSS` - Vue Single File Component with PostCSS
- `vueCSS` - Vue Single File Component with CSS
- `vueStylus` - Vue Single File Component with Stylus
- `vueTypeScript` - Vue Single File Component with TypeScript
- `vueTypeScriptClass` - Vue Single File Component with Class based TypeScript format
- `vueNoStyle` - Vue Single File Component with No Style
- `vueTemplate` - Vue Template element
- `vueScript` - Vue Script element
- `vueStyle`/`styleLang` - Vue Style element

### JavaScript/TypeScript/Vue 🌿

#### Import

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
- `store.getters` - [this.]store.getters
- `store.state` - [this.]store.state
- `store.commit()` / `sc` - [this.]store.commit(type, payload, options)
- `store.dispatch()` / `sd` - [this.]store.dispatch(type, payload)
- `store.dispatch()` / `sdp` - [this.]store.dispatch(type, payload), promise
- `store.replaceState()` - [this.]store.replaceState(state)
- `store.watch()` - [this.]store.watch(getter, cb, options)
- `store.subscribe()` - [this.]store.subscribe(fn, options)
- `store.subscribeAction()` - [this.]store.subscribeAction(fn, options)
- `store.subscribeAction()` - [this.]store.subscribeAction(object)
- `store.registerModule()` - [this.]store.registerModule(path, rawModule, options)
- `store.unregisterModule()` - [this.]store.unregisterModule(path)
- `store.hasModule()` - [this.]store.hasModule(path)
- `store.hotUpdate()` - [this.]store.hotUpdate(newOptions)


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

Let's try `pDDR`, Other parts can be operated in the same way.

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

#### Transition

- `beforeEnterEvent` / `transitionBeforeEnterEvent` - before-enter
- `enterEvent` / `transitionEnterEvent` - enter
- `afterEnterEvent` / `transitionAfterEnterEvent` - after-enter
- `enterCancelledEvent` / `transitionEnterCancelledEvent` - enter-cancelled
- `beforeLeaveEvent` / `transitionBeforeLeaveEvent` - before-leave
- `leaveEvent` / `transitionLeaveEvent` - leave
- `afterLeaveEvent` / `transitionAfterLeaveEvent` - after-leave
- `leaveCancelledEvent` / `transitionLeaveCancelledEvent` - leave-cancelled
- `beforeAppearEvent` / `transitionBeforeAppearEvent` - before-appear
- `appearEvent` / `transitionAppearEvent` - appear
- `afterAppearEvent` / `transitionAfterAppearEvent` - after-appear
- `appearCancelledEvent` / `transitionAppearCancelledEvent` - appear-cancelled


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

### HTML 🌴

#### Style & Class

- `vClass` - `:class="{ 'class-name': expression }"`, Class binding: object syntax inline
- `vClass` - `:class="classObject"`, Class binding: object syntax
- `vClass` - `:class="[classObject]"`, Class binding: apply a list of classes
- `vClass` - `:class="[expression ? 'class-name' : '', classObject]"`, Class binding: with a ternary expression
- `vClass` - `:class="[classObject, { 'class-name': expression }]"`, Class binding: multiple conditional classes
- `vStyle` - `:style="{ 'css-property': 'value', cssProperty: `${styleValue}px` }"`, Style binding: object syntax inline
- `vStyle` - `:style="styleObject"`, Style binding: object syntax
- `vStyle` - `:style="[baseStyles, overridingStyles]"`, Style binding: multiple styles

#### Directives

- `template` - template
- `templateFunctional` - functional template
- `xtemplate` - x-template
- `vFor` - `v-for="(item, index) in items" :key="index"`, Vue v-for
- `vForWithoutKey` - `v-for="item in items"`, Vue v-for, Without Key
- `vIf` - `v-if="condition"`, Vue v-if
- `vElse` - `v-else`, Vue v-else
- `vElseIf` - `v-else-if="condition"`, Vue v-else-if
- `vIfWithKey_UNSAFE` - `v-if="condition" key="{feature}"`, Vue v-if, With Key, **Vue 3 DEPRECATED!**
- `vElseWithKey_UNSAFE` - `v-else key="{feature}"`, Vue v-else, With Key, **Vue 3 DEPRECATED!**
- `vElseIfWithKey_UNSAFE` - `v-else-if="condition" key="{feature}"`, Vue v-else-if, With Key, **Vue 3 DEPRECATED!**
- `vShow` - `v-show="condition"`, Vue v-show
- `vText` - `v-text="text"`, Vue v-text
- `vFilter_UNSAFE` - `:text-content.prop="text | filter"`, Vue v-bind filter, **Vue 3 REMOVED!**
- `vHtml` - `v-html="html"`, Vue v-html
- `vModel` - `v-model="value"`, Vue v-model
- `vOn` - `@click="handler(arg, $event)"`, v-on event/listener
- `vOnLonghand` - `v-on:click="handler(arg, $event)"`, v-on Longhand
- `vOnDynamic` - `@[event]="handler(arg, $event)"`, v-on dynamic event
- `vOnStopPropagation` - `vOnStopPropagation`, v-on stop propagation
- `vOnPreventDefault` - `@click.prevent="handler(arg, $event)"`, v-on prevent default
- `vOnStopPropagationPreventDefault` - `@click.stop.prevent="handler(arg, $event)"`, v-on stop propagation and prevent default
- `vOnKeyAlias` - `@keyup.enter="handler(arg, $event)"`, v-on key modifier using keyAlias
- `vOnKeyCode_UNSAFE` - `@keyup.13="handler(arg, $event)"`, v-on key modifier using keyCode, **Vue 3 DEPRECATED!**
- `vOnOnce` - `@click.once="handler(arg, $event)"`, v-on triggered at most once
- `vOnObject` - `v-on="{ mousedown: handler(arg, $event), mouseup: handler(arg, $event) }"`, v-on object syntax
- `vBind` - `:attribute="value"`, Vue v-bind
- `vBindLonghand` - `v-bind:attribute="value"`, Vue v-bind Longhand
- `vBindDynamic` - `:[attribute]="value"`, Vue v-bind dynamic directive
- `vAttrs` - `"v-bind="$attrs"`, Vue v-bind $attrs
- `vOnce` - `v-once `, Vue v-once
- `vPre` - `v-pre `, Vue v-pre
- `vCloak` - `v-cloak `, Vue v-cloak
- `vEmit` - `@event="$emit('event-name', $event.target.value)"`, $emit
- `ref` - `ref="reference"`
- `key` - `:key="number|string|boolean|symbol"`

#### Built-in Components

- `component` - `<component :is="componentId"></component>`
- `keepAlive` - `<keep-alive></keep-alive>`

#### Slots

- `slotElement` - `<slot>` Element
- `slotElementScope` - `<slot>` Element, Scoped Slots
- `vSlot` - v-slot
- `vSlotScope` - v-slot, Scoped Slots
- `vSlotLonghand` - v-slot, Longhand
- `vSlotScopeLonghand` - v-slot, Scoped Slots, Longhand
- `UNSAFE_slot` - UNSAFE!!! Slot Deprecated
- `UNSAFE_slotScope` - UNSAFE!!! Slot Deprecated, Scope Removed
- `UNSAFE_slotSlotScope` - UNSAFE!!! Slot Deprecated, slotScope Deprecated

#### Transitions

- `transition` - Vue Transition Component
- `transition` - Vue Transition Component with JavaScript Hooks
- `transitionGroup` - Vue transition-group Component

##### Custom Transition Classes

- `enterClass` / `transitionEnterClass` - enter-class
- `enterActiveClass` / `transitionEnterActiveClass` - enter-active-class
- `enterToClass` / `transitionEnterToClass` - enter-to-class
- `leaveClass` / `transitionLeaveClass` - leave-class
- `leaveToClass` / `transitionLeaveToClass` - leave-to-class
- `leaveActiveClass` / `transitionLeaveActiveClass` - leave-active-class
- `appearClass` / `transitionAppearClass` - appear-class
- `appearToClass` / `transitionAppearToClass` - appear-to-class
- `appearActiveClass` / `transitionAppearActiveClass` - appear-active-class

##### JavaScript Hooks

- `beforeEnterHook`/`transitionBeforeEnterHook` → `@before-enter='beforeEnter'`
- `enterHook`/`transitionEnterHook` → `@enter='enter'`
- `afterEnterHook`/`transitionAfterEnterHook` → `@after-enter='afterEnter'`
- `enterCancelledHook`/`transitionEnterCancelledHook` → `@enter-cancelled='enterCancelled'`
- `beforeLeaveHook`/`transitionBeforeLeaveHook` → `@before-leave='beforeLeave'`
- `leaveHook`/`transitionLeaveHook` → `@leave='leave'`
- `afterLeaveHook`/`transitionAfterLeaveHook` → `@after-leave='afterLeave'`
- `leaveCancelledHook`/`transitionLeaveCancelledHook` → `@leave-cancelled='leaveCancelled'`
- `beforeAppearHook`/`transitionBeforeAppearHook` → `@before-appear='beforeAppear'`
- `appearHook`/`transitionAppearHook` → `@appear='appear'`
- `afterAppearHook`/`transitionAfterAppearHook` → `@after-appear='afterAppear'`
- `appearCancelledHook`/`transitionAppearCancelledHook` → `@appear-cancelled='appearCancelled'`


#### Vue Router

- `routerView` - `<router-view></router-view>`, Router View;
- `routerViewNamed` - `<router-view name="viewFeature"></router-view>`, Named Router View;
- `routerLink` - `<router-link to="">path</router-link>`, Router link with literal string;
- `routerLink` - `<router-link :to="">path</router-link>`, Router link using v-bind;
- `routerLinkPath` - `<router-link :to="{ path: 'pathname' }">pathname</router-link>`, Router link to path;
- `routerLinkParams` - `<router-link :to="{ path: 'pathname', params: { property: 'value' } }">path</router-link>`, Router link to path with params;
- `routerLinkQuery` - `<router-link :to="{ path: 'pathname', query: { property: 'value' } }">path</router-link>`, Router link to path with query;
- `routerLinkAppend` - `<router-link :to="{ path: 'pathname' }" append>path</router-link>`, Router link to path using append mode;
- `routerLinkReplace` - `<router-link :to="{ path: 'pathname' }" replace>path</router-link>`, Router link to path using replace mode;
- `routerLinkNamedRoute` - `<router-link :to="{ name: 'routename' }">path</router-link>`, Router link to named route;
- `routerLinkNamedRouteParams` - `<router-link :to="{ name: 'routename', params: { property: 'value' } }">path</router-link>`, Router link to named route with params;
- `routerLinkNamedRouteQuery` - `<router-link :to="{ name: 'routename', query: { property: 'value' } }">path</router-link>`, Router link to named route with query;
- `routerParams` - `params: { property: 'value' }`, Router with params;
- `routerQuery` - `query: { property: 'value' }`, Router with query;
- `routerActiveClass` - `active-class="router-link-active"`, Router active-class;
- `routerExact` - `exact`, Router with exact match;
- `routerExactActiveClass` - `exact-active-class="router-link-exact-active"`, Router exact-active-class;
- `routerAriaCurrentValue` - `aria-current-value="page"`, Router aria-current-value;
- `routerTag` - `tag="a"`, Router tag;


### CSS 🌷

- `v-cloak`
- `enterCSS`/ `transitionEnterCSS`  → `.feature-enter {}`
- `enterActiveCSS`/`transitionEnterActiveCSS`  → `.feature-enter-active {}`
- `enterToCSS`/ `transitionEnterToCSS`  → `.feature-enter-to {}`
- `leaveCSS`/ `transitionLeaveCSS`  → `.feature-leave {}`
- `leaveToCSS`/ `transitionLeaveToCSS`  → `.feature-leave-to {}`
- `leaveActiveCSS`/`transitionLeaveActiveCSS`  → `.feature-leave-active {}`
- `appearCSS`/ `transitionAppearCSS`  → `.feature-appear {}`
- `appearToCSS`/ `transitionAppearToCSS`  → `.feature-appear-to {}`
- `appearActiveCSS`/`transitionAppearActiveCSS`  → `.feature-appear-active {}`

---

## File Name

View "Style Guide" [Priority B Rules: Strongly Recommended (Improving Readability)](https://v3.vuejs.org/style-guide/#priority-b-rules-strongly-recommended-improving-readability).

- foo-bar`${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/g}`, .vue  →  `name: FooBar`;
- foo-bar`${TM_FILENAME_BASE}`, .vue  →  `name: foo-bar`;
- foo-bar`${TM_DIRECTORY}`, /index.vue  →  `name: foo-bar`;


## License 📃

MIT License

---

TODO: vue-ssr


**Donate**

![xianghongai@gmail.com](https://raw.githubusercontent.com/caringrun/assets/master/donate.png)