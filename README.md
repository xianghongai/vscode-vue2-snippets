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

## Features 🦢



### Lifecycle Hooks (Options API)

```txt
+------------------------+-----------------------+-------------------+
| Prefix                 | VS Code Suggest Match | Snippet           |
+------------------------+-----------------------+-------------------+
| option-beforeCreate()  | opbc                  | beforeCreate() {  |
|                        |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-created()       | opcr                  | created() {       |
|                        |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-beforeMount()   | opbm                  | beforeMount() {   |
|                        |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-mounted()       | opmu                  | mounted() {       |
|                        |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-beforeUpdate()  | opbu                  | beforeUpdate() {  |
|                        |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-updated()       | opu                   | updated() {       |
|                        |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-activated()     | opac                  | activated() {     |
|                        |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-deactivated()   | opdeac                | deactivated() {   |
|                        |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-beforeDestroy() | opbd                  | beforeDestroy() { |
|                        |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
| option-destroyed()     | opdes                 | destroyed() {     |
|                        |                       |                   |
|                        |                       | },                |
+------------------------+-----------------------+-------------------+
```

### Lifecycle Hooks (Composition API)

```txt
+-------------------------------------------------------------------+
| Prefix          | VS Code Suggest Match | Snippet                 |
+-----------------+-----------------------+-------------------------+
| onBeforeMount   | obm                   | onBeforeMount(() => {   |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onMounted       | omo                   | onMounted(() => {       |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onBeforeUpdate  | obup                  | onBeforeUpdate(() => {  |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onUpdated       | oup                   | onUpdated(() => {       |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onBeforeUnmount | obum                  | onBeforeUnmount(() => { |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onUnmounted     | oum                   | onUnmounted(() => {     |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onActivated     | oac                   | onActivated(() => {     |
|                 |                       |                         |
|                 |                       | });                     |
+-----------------+-----------------------+-------------------------+
| onDeactivated   | oda                   | onDeactivated(() => {   |
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
