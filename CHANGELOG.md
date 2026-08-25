# Changelog

All notable changes to the **Vue 2 Snippets** extension are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Each entry lists only the headline change per release — see git history/tags for full detail. Patch releases that only touched documentation or the build are folded into the entry above them.

## [2.5.1] - 2026-08-25

- Internal only, no change to the published snippets: migrated the toolchain to pnpm + [mise](https://mise.jdx.dev/), reformatted `src/` with Prettier, and reworked packaging (allow-list `.vscodeignore`, corrected `engines.vscode`, and a `vscode:prepublish` hook so `snippets/` is always regenerated before publish)

## [2.5.0] - 2024-11-26

- Refinements across the Composition API and SFC snippets

## [2.4.0] - 2024-11-13

- Reorganized the Composition API snippets to mirror the official API reference chapters, and expanded the global API and reactivity sections (2.4.1 and 2.4.2 followed same-day with a fix and documentation)

## [2.3.0] - 2024-07-08

- Updates across the built-in directives, Composition API, and SFC templates

## [2.2.0] - 2024-03-04

- Expanded the Composition API snippet set (2.2.1–2.2.7 followed with small fixes and documentation cleanups)

## [2.1.0] - 2024-03-04

- Added the Transition section — transition classes, transition events, and the CSS counterparts

## [2.0.1] - 2024-03-03

- Major refactor: Composition API support (via `@vue/composition-api`) alongside the Options API, `src/` reorganized by topic, and the built-in directives/components/special-elements split into dedicated files

## [1.3.0] - 2022-11-28

- Vuex snippets moved to a separate repository (1.3.1 and 1.3.2 followed with title and snippet updates)

## [1.2.0] - 2022-11-26

- Added `import` snippets for service/util/constant/config; in 1.2.1 they moved to `vscode-vue-basic-snippets`

## [1.1.0] - 2021-09-30

- Broad snippet revision; 1.1.1 simplified the prefixes

## [1.0.0] - 2021-05-09

- Initial release, followed through 1.0.8 by script upgrades and additions such as `await this.$nextTick()`
