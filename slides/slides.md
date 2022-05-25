---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: true
# persist drawings in exports and build
drawings:
  persist: false
---

# WIP

## Hook:
  * We all love to build Vue applications (right?) - connect "somehow" to amazing talks from before
  * Not always a green field - not always SPAs - maybe LAMP, maybe Java based monoliths (traditional server-rendered)
  * Actually, most of the projects are "legacy"
    * jQuery/MooTools/...
  * Sometimes not migratable to SPAs (time/budget/experience?)
  * But still we want to add interactivity to such projects every now and then as well
    * With a modern approach!

## Progressive Enhancement

* Why not use Vue directly?
  * Build step
  * Toolchain setup to unleash full potential
  * X kB
  * Optimizations
  * Too powerful/too much new to learn

## `petite-vue`

* No VDOM, thus super small (X kB)
* Can controls specific areas of the page

### Tech

* v-scope
* Auto init
* Show component examples

### Limitations

* No `ref` nor `computed`
* No `render` functions (due to missing VDOM)
* SPA features like transitions, teleports, suspense and more

### Live coding?

3. `petite-vue` vs. `alpine`?

* Inspired by alpine
* Both powered by VueJS reactivity

<!---

https://twitter.com/youyuxi/status/1410759893359874050

Vanilla.js 0 kB?

https://twitter.com/stauffermatt/status/1403798390585053190

-->