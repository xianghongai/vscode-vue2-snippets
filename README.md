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

### Props

```txt

```

### Lifecycle Hooks (Options API)

只要**理解** `ol` 是 <strong><u style="color: red;">O</u></strong>ptions API <strong><u style="color: red;">L</u></strong>ifecycle Hooks` 的缩写，并**记忆** Vue2 生命周期钩子，然后就能释放你的能量了。

```txt
+------------------------+-----------------------+-------------------+
| Prefix                 | VS Code Suggest Match | Snippet           |
+------------------------+-----------------------+-------------------+
| option-beforeCreate()  | opbc                  | beforeCreate() {  |
| olbc                   |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-created()       | opcr                  | created() {       |
| olc                    |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-beforeMount()   | opbm                  | beforeMount() {   |
| olbm                   |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-mounted()       | opmu                  | mounted() {       |
| olm                    |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-beforeUpdate()  | opbu                  | beforeUpdate() {  |
| olbu                   |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-updated()       | opu                   | updated() {       |
| olu                    |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-activated()     | opac                  | activated() {     |
| ola                    |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-deactivated()   | opdeac                | deactivated() {   |
| olda                   |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-beforeDestroy() | opbd                  | beforeDestroy() { |
| olbd                   |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-destroyed()     | opdes                 | destroyed() {     |
| old                    |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
```

### Lifecycle Hooks (Composition API)

```txt
+-------------------------------------------------------------------+
| Prefix          | VS Code Suggest Match | Snippet                 |
+-----------------+-----------------------+-------------------------+
| onBeforeMount   | onbm                  | onBeforeMount(() => {   |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onMounted       | onm                   | onMounted(() => {       |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onBeforeUpdate  | onbup                 | onBeforeUpdate(() => {  |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onUpdated       | onup                  | onUpdated(() => {       |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onBeforeUnmount | onbu                  | onBeforeUnmount(() => { |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onUnmounted     | onum                  | onUnmounted(() => {     |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onActivated     | ona                   | onActivated(() => {     |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onDeactivated   | onda                  | onDeactivated(() => {   |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
```

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
