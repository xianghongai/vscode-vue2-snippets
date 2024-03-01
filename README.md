<p>
  <h1 align="center">Vue 2 Snippet (Visual Studio Code)</h1>
</p>

<p align="center">
  <a href="https://github.com/xianghongai/vscode-vue2-snippets">
    <img src="https://img.shields.io/github/repo-size/xianghongai/vscode-vue2-snippets?color=4ac51c&style=plastic&?cacheSeconds=3600">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=nicholashsiang.vscode-vue2-snippets">
    <img src="https://img.shields.io/visual-studio-marketplace/v/nicholashsiang.vscode-vue2-snippets?color=%234ac51c&style=plastic&?cacheSeconds=3600">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=nicholashsiang.vscode-vue2-snippets">
    <img src="https://img.shields.io/visual-studio-marketplace/d/nicholashsiang.vscode-vue2-snippets?color=4ac51c&style=plastic&?cacheSeconds=3600">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=nicholashsiang.vscode-vue2-snippets">
    <img src="https://img.shields.io/visual-studio-marketplace/r/nicholashsiang.vscode-vue2-snippets?color=4ac51c&style=plastic&?cacheSeconds=3600">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=nicholashsiang.vscode-vue2-snippets">
    <img src="https://img.shields.io/github/license/xianghongai/vscode-vue2-snippets?color=4ac51c&style=plastic&?cacheSeconds=3600">
  </a>
</p>

## Introduction 📚



For example, `beforeCreate` has two triggering methods:

1. Prefix Directly：`olbc` = <strong><u style="color: red;">O</u></strong>ptions API <strong><u style="color: red;">L</u></strong>ifecycle Hooks <strong><u style="color: red;">b</u></strong>efore<strong><u style="color: red;">C</u></strong>reate()
2. Suggest Match：`opbc` = <strong><u style="color: red;">Op</u></strong>tions API <strong><u style="color: red;">b</u></strong>efore<strong><u style="color: red;">C</u></strong>reate()

Why is Prefix `olbc` instead of `opbc`? Because the `op*` prefix will have many conflicts, and using the `ol*` prefix can limit the range.

Abbreviate prefixes are for often used.

--

为提升编码效率，本插件提供了 Vue 2 的代码片段，包括 Options API 和 Composition API，同时包含 `@vue/composition-api` 中的 API；

为了减少记忆负担、理解成本，本插件提供了缩写前缀 (部分)，以及联想匹配前缀 (主要)，方便用户快速输入代码片段。

比如，`beforeCreate` 有两种触发方式：

1. 直接生成 (Prefix)：`olbc` = <strong><u style="color: red;">O</u></strong>ptions API <strong><u style="color: red;">L</u></strong>ifecycle Hooks <strong><u style="color: red;">b</u></strong>efore<strong><u style="color: red;">C</u></strong>reate()
2. 联想匹配 (Suggest Match)：`opbc` = <strong><u style="color: red;">Op</u></strong>tions API <strong><u style="color: red;">b</u></strong>efore<strong><u style="color: red;">C</u></strong>reate()

Prefix 为什么是 `olbc` 而不是 `opbc`？因为 `op*` 前缀会有很多冲突，而使用 `ol*` 前缀能限定为范围；

仅高频常用代码提供**缩写**前缀。

## Features 🦢

### Options API

| Prefix                               | VS Code Suggest Match | Snippet                                                                                                                                                                                               |
|--------------------------------------|-----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `option-name`                        |                       | name: 'FileName',                                                                                                                                                                                     |
| `option-components` / `ocs`          |                       | components: { Feature },                                                                                                                                                                              |
| `option-directives`                  |                       | directives: {<br>&nbsp;&nbsp;<br>},                                                                                                                                                                   |
| `option-props` / `ops`               | `opps`                | props: {<br>&nbsp;&nbsp;<br>},                                                                                                                                                                        |
| `option-provide()` / `ope`           |                       | provide() {<br>&nbsp;&nbsp;return {<br>&nbsp;&nbsp;&nbsp;&nbsp;property: 'value',<br>&nbsp;&nbsp;};<br>},                                                                                             |
| `option-inject` / `oit`              |                       | inject: ['property'],                                                                                                                                                                                 |
| `option-data()` / `od`               | `opd`                 | data() {<br>&nbsp;&nbsp;return {<br>&nbsp;&nbsp;&nbsp;&nbsp;property: 'value',<br>&nbsp;&nbsp;};<br>},                                                                                                |
| `option-computed` / `oc`             | `opc`                 | computed: {<br>&nbsp;&nbsp;property() {<br>&nbsp;&nbsp;&nbsp;&nbsp;return this.property;<br>&nbsp;&nbsp;},<br>},                                                                                      |
| `computed-property` / `cp`           |                       | property() {<br>&nbsp;&nbsp;return this.property;<br>},                                                                                                                                               |
| `computed-property-get-set` / `cpgs` |                       | property: {<br>&nbsp;&nbsp;get() {<br>&nbsp;&nbsp;&nbsp;&nbsp;return this.value;<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;set(value) {<br>&nbsp;&nbsp;&nbsp;&nbsp;this.value = value;<br>&nbsp;&nbsp;},<br>}, |
| `option-watch` / `ow`                | `opw`                 | watch: {<br>&nbsp;&nbsp;<br>},                                                                                                                                                                        |
| `option-methods` / `om`              | `opm`                 | methods: {<br>&nbsp;&nbsp;methodName() {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>},                                                                                                          |
| `methods-property` / `mp`            |                       | methodName() {<br>&nbsp;&nbsp;<br>},                                                                                                                                                                  |
| `option-emits`                       |                       | emits: \['eventName'\],                                                                                                                                                                               |
| `option-expose`                      |                       | expose: \['publicMethod'\],                                                                                                                                                                           |
| `option-render`                      |                       | render(h, context) {<br>&nbsp;&nbsp;return h('tag', []);<br>},                                                                                                                                        |

### Props Property

1. 直接生成 (Prefix)：`ps` = <strong><u style="color: red;">P</u></strong>rops, <strong><u style="color: red;">S</u></strong>tring.
2. 联想匹配 (Suggest Match)：`pssdr` = <strong><u style="color: red;">P</u></strong>rop<strong><u style="color: red;">s</u></strong>, <strong><u style="color: red;">S</u></strong>tring, <strong><u style="color: red;">d</u></strong>efault, <strong><u style="color: red;">r</u></strong>equired.

不同类型以此类推：

- <strong><u style="color: red;">S</u></strong>tring，
- <strong><u style="color: red;">N</u></strong>umber，
- <strong><u style="color: red;">B</u></strong>oolean，
- <strong><u style="color: red;">A</u></strong>rray，
- <strong><u style="color: red;">O</u></strong>bject，
- <strong><u style="color: red;">D</u></strong>ate，
- <strong><u style="color: red;">F</u></strong>unction，
- <strong><u style="color: red;">S</u></strong>ymbol，
- <strong><u style="color: red;">P</u></strong>romise。

| Prefix                                   | VS Code Suggest Match | Snippet                                                                                                          |
|------------------------------------------|-----------------------|------------------------------------------------------------------------------------------------------------------|
| `props-String` / `ps`                    | `pss`                 | property: String,                                                                                                |
| `props-String-default` / `psd`           | `pssd`                | property: {<br>&nbsp;&nbsp;type: String,<br>&nbsp;&nbsp;default: undefined,<br>},                                |
| `props-String-required` / `psr`          | `pssr`                | property: {<br>&nbsp;&nbsp;type: String,<br>&nbsp;&nbsp;required: true,<br>},                                    |
| `props-String-default-required` / `psdr` | `pssdr`               | property: {<br>&nbsp;&nbsp;type: String,<br>&nbsp;&nbsp;default: undefined,<br>&nbsp;&nbsp;required: true,<br>}, |
| ...                                      |                       |                                                                                                                  |

###  Watch Property (Options API)

1. 直接生成 (Prefix)：`wp` = <strong><u style="color: red;">w</u></strong>atch-<strong><u style="color: red;">p</u></strong>roperty。
2. 联想匹配 (Suggest Match)：`wpdi` = <strong><u style="color: red;">w</u></strong>atch-<strong><u style="color: red;">p</u></strong>roperty-<strong><u style="color: red;">d</u></strong>eep-<strong><u style="color: red;">i</u></strong>mmediate。

| Prefix                                   | VS Code Suggest Match | Snippet                                                                                                                                                                 |
|------------------------------------------|-----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `watch-property` / `wp`                  |                       | property (newValue, oldValue) {<br>&nbsp;&nbsp;<br>},                                                                                                                   |
| `watch-property-deep` / `wpd`            |                       | property: {<br>&nbsp;&nbsp;deep: true,<br>&nbsp;&nbsp;handler(newValue, oldValue) {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>},                                 |
| `watch-property-immediate` / `wpi`       |                       | property: {<br>&nbsp;&nbsp;immediate: true,<br>&nbsp;&nbsp;handler(newValue, oldValue) {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>},                            |
| `watch-property-deep-immediate` / `wpdi` |                       | property: {<br>&nbsp;&nbsp;deep: true,<br>&nbsp;&nbsp;immediate: true,<br>&nbsp;&nbsp;handler(newValue, oldValue) {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>}, |

### Watch (Composition API)

1. 联想匹配 (Suggest Match)：`wps` = <strong><u style="color: red;">w</u></strong>atch-<strong><u style="color: red;">p</u></strong>rop<strong><u style="color: red;">s</u></strong>。
2. 联想匹配 (Suggest Match)：`wim` = <strong><u style="color: red;">w</u></strong>atch-<strong><u style="color: red;">im</u></strong>mediate。

| Prefix                           | VS Code Suggest Match | Snippet                                                                                                                                                                                                                                                             |
|----------------------------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `watch-props`                    | `wps`                 | watch(<br>&nbsp;&nbsp;() => props.property,<br>&nbsp;&nbsp;async (newValue, oldValue) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>);                                                                                                                      |
| `watch-props-deep`               | `wpsd`                | watch(<br>&nbsp;&nbsp;() => props.property,<br>&nbsp;&nbsp;async (newValue, oldValue) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;deep: true,<br>&nbsp;&nbsp;}<br>);                                             |
| `watch-props-immediate`          | `wpsi`                | watch(<br>&nbsp;&nbsp;() => props.property,<br>&nbsp;&nbsp;async (newValue, oldValue) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;immediate: true,<br>&nbsp;&nbsp;}<br>);                                        |
| `watch-props-deep-immediate`     | `wpsdi`               | watch(<br>&nbsp;&nbsp;() => props.property,<br>&nbsp;&nbsp;async (newValue, oldValue) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;deep: true,<br>&nbsp;&nbsp;&nbsp;&nbsp;immediate: true,<br>&nbsp;&nbsp;}<br>); |
| `watch-props-immediate-multiple` | `wpsimu`              | watch(<br>&nbsp;&nbsp;[() => props.property1, () => props.property2],<br>&nbsp;&nbsp;async ([property1, property2]) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;immediate: true,<br>&nbsp;&nbsp;}<br>);          |
| `watch`                          |                       | watch(<br>&nbsp;&nbsp;source,<br>&nbsp;&nbsp;async (newValue, oldValue) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>);                                                                                                                                    |
| `watch-deep`                     | `wd`                  | watch(<br>&nbsp;&nbsp;source,<br>&nbsp;&nbsp;async (newValue, oldValue) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;deep: true,<br>&nbsp;&nbsp;}<br>);                                                           |
| `watch-immediate`                | `wim`                 | watch(<br>&nbsp;&nbsp;source,<br>&nbsp;&nbsp;async (newValue, oldValue) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;immediate: true,<br>&nbsp;&nbsp;}<br>);                                                      |
| `watch-deep-immediate`           | `wdi`                 | watch(<br>&nbsp;&nbsp;source1,<br>&nbsp;&nbsp;async (newValue, oldValue) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;deep: true,<br>&nbsp;&nbsp;&nbsp;&nbsp;immediate: true,<br>&nbsp;&nbsp;}<br>);              |
| `watch-immediate-multiple`       | `wimu`                | watch(<br>&nbsp;&nbsp;[source1, source2],<br>&nbsp;&nbsp;async ([nextSource1, nextSource2], [prevSource1, prevSource2]) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;immediate: true,<br>&nbsp;&nbsp;}<br>);      |
| `watchEffect`                    | `wef`                 | watchEffect(async () => {<br>&nbsp;&nbsp;<br>});                                                                                                                                                                                                                    |
| `watchPostEffect`                | `wpef`                | watchPostEffect(async () => {<br>&nbsp;&nbsp;<br>});                                                                                                                                                                                                                |
| `watchSyncEffect`                | `wsef`                | watchSyncEffect(() => {<br>&nbsp;&nbsp;<br>});                                                                                                                                                                                                                      |

### Computed

| Prefix                               | VS Code Suggest Match | Snippet                                                                                                                                                                                           |
|--------------------------------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `computed-property` / `cp`           |                       | property() {<br>&nbsp;&nbsp;return this.property;<br>},                                                                                                                                           |
| `computed-property-get-set` / `cpgs` |                       | property: {<br>&nbsp;&nbsp;get() {<br>&nbsp;&nbsp;&nbsp;&nbsp;return this.value;<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;set(val) {<br>&nbsp;&nbsp;&nbsp;&nbsp;this.value = val;<br>&nbsp;&nbsp;},<br>}, |
| `compute`                            |                       | const feature = computed(() => state.value);                                                                                                                                                      |
| `computed-get-set`                   |                       | const feature = computed({<br>&nbsp;&nbsp;get: () => state.value,<br>&nbsp;&nbsp;set: (newValue) => {<br>&nbsp;&nbsp;&nbsp;&nbsp;state.value = newValue;<br>&nbsp;&nbsp;},<br>});                 |

### Lifecycle Hooks (Options API)

只要**理解** `ol` 是 <strong><u style="color: red;">O</u></strong>ptions API <strong><u style="color: red;">L</u></strong>ifecycle Hooks` 的缩写，并**记忆** Vue2 生命周期钩子，然后就能释放你的能量了。

| Prefix                             | VS Code Suggest Match | Snippet                                 |
|------------------------------------|-----------------------|-----------------------------------------|
| `option-beforeCreate()` / `olbc`   | `opbc`                | beforeCreate() {<br>&nbsp;&nbsp;<br>},  |
| `option-created()` / `olc`         | `opcr`                | created() {<br>&nbsp;&nbsp;<br>},       |
| `option-beforeMount()` / `olbm`    | `opbm`                | beforeMount() {<br>&nbsp;&nbsp;<br>},   |
| `option-mounted()` / `olm`         | `opmu`                | mounted() {<br>&nbsp;&nbsp;<br>},       |
| `option-beforeUpdate()` / `olbu`   | `opbu`                | beforeUpdate() {<br>&nbsp;&nbsp;<br>},  |
| `option-updated()` / `olu`         | `opu`                 | updated() {<br>&nbsp;&nbsp;<br>},       |
| `option-activated()` / `ola`       | `opac`                | activated() {<br>&nbsp;&nbsp;<br>},     |
| `option-deactivated()` / `olda`    | `opdeac`              | deactivated() {<br>&nbsp;&nbsp;<br>},   |
| `option-beforeDestroy()` / `olbd`  | `opbd`                | beforeDestroy() {<br>&nbsp;&nbsp;<br>}, |
| `option-destroyed()` / `old`       | `opdes`               | destroyed() {<br>&nbsp;&nbsp;<br>},     |
| `async-option-created()` / `asolc` | `asopcr`              | async created() {<br>&nbsp;&nbsp;<br>}, |
| `async-option-mounted()` / `asolm` | `asopmu`              | async mounted() {<br>&nbsp;&nbsp;<br>}, |

### Lifecycle Hooks (Composition API)

| Prefix            | VS Code Suggest Match | Snippet                                        |
|-------------------|-----------------------|------------------------------------------------|
| `onBeforeMount`   | `onbm`                | onBeforeMount(() => {<br>&nbsp;&nbsp;<br>});   |
| `onMounted`       | `onm`                 | onMounted(() => {<br>&nbsp;&nbsp;<br>});       |
| `onBeforeUpdate`  | `onbup`               | onBeforeUpdate(() => {<br>&nbsp;&nbsp;<br>});  |
| `onUpdated`       | `onup`                | onUpdated(() => {<br>&nbsp;&nbsp;<br>});       |
| `onBeforeUnmount` | `onbu`                | onBeforeUnmount(() => {<br>&nbsp;&nbsp;<br>}); |
| `onUnmounted`     | `onum`                | onUnmounted(() => {<br>&nbsp;&nbsp;<br>});     |
| `onActivated`     | `ona`                 | onActivated(() => {<br>&nbsp;&nbsp;<br>});     |
| `onDeactivated`   | `onda`                | onDeactivated(() => {<br>&nbsp;&nbsp;<br>});   |
| `async-onMounted` | `asonm`               | onMounted(async () => {<br>&nbsp;&nbsp;<br>}); |

### Instance Properties & Methods

| Prefix              | VS Code Suggest Match | Snippet                                                            |
|---------------------|-----------------------|--------------------------------------------------------------------|
| `vm.nextTick`       | `vmnt`                | this.$<u>n</u>ext<u>T</u>ick().then(() => {<br>&nbsp;&nbsp;<br>}); |
| `await-vm.nextTick` | `awvmnt`              | <u>aw</u>ait this.$<u>n</u>ext<u>T</u>ick();                       |
| `vm.emit`           | `vmem`                | this.$<u>em</u>it('event-name', param);                            |

### Vue Route v3.x



## Supported languages (file extensions)

- JavaScript (`.js`)
- TypeScript (`.ts`)
- HTML (`.html`)
- Vue (`.vue`)

## The `UNSAFE` prefix/suffix

`UNSAFE_x`，`prefix`, Indicates that it is deprecated in the **current** version.

`x_UNSAFE`，`suffix`, Indicates that it has been deprecated in **future** versions.

## Resources 🤞

- [Vue 3 Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue3-snippets), For Vue 3.
- [Pinia Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-pinia-snippets), For Pinia.
- [VueX Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vuex-snippets), For VueX.
- [JavaScript Code Snippet](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-javascript-snippet), Reference MDN documentation.
- [JavaScript Comment Snippet](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-javascript-comment), Reference JSDOC, ESDOC documentation.

## License 📃

MIT License

---

**Donate**

![xianghongai@gmail.com](https://raw.githubusercontent.com/caringrun/assets/master/donate.png)
