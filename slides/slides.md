---
theme: ./theme
website: 'lichter.io'
handle: 'TheAlexLichter'
favicon: 'https://lichter.io/img/me@2x.jpg'
highlighter: shiki
lineNumbers: true
layout: intro
---

<h1>petite-<span class="text-[#41b883]">vue</span> <logos-vue class="-ml-2 text-2xl" /></h1>

<h2>Progressively enhancing <span class="text-[#41b883]">every</span> application?</h2>

<br><br><br><br>

### Vue.js Amsterdam 2022

---
layout: two-cols
heading: About me
---

<template v-slot:default>
<div class="flex flex-col justify-center items-center h-full">
<img
  class="w-75 rounded-full"
  src="https://lichter.io/img/me@2x.webp"
  />
  <h2 class="mt-4">Alexander Lichter</h2>
</div>
</template>

<template v-slot:right>
<VClicks class="space-y-2 mt-10 text-xl h-full">

* <mdi-account-check class="text-green-100" /> Web Development Consultant
* <mdi-microphone /> Speaker & Instructor
* <logos-nuxt-icon /> Nuxt.js Maintainer
* <mdi-twitter class="text-blue-400" /> @TheAlexLichter
* <mdi-web /> [https://lichter.io](https://lichter.io)

</VClicks>
</template>

---
layout: intro
---

# When we build with <logos-vue />...
# ...we mostly develop SPAs

---
layout: intro
---

# But how many percent of all websites are SPAs?

<img>

<!-- 
SPA = Not only Vue

Ask the audience to shout the number
-->

---

# We don't know how many SPAs exist out there!

---

# We <mdi-heart class="text-red-500"/> writing <logos-vue /> applications, right?

<VClicks>

* But there are so many situations where we can't
* Test

</VClicks>

---

# WIP

## Hook:
  * We all love to build Vue applications (right?) - connect "somehow" to amazing talks from before
  * But how many % of the websites are Single Page Applications (not only Vue)?
  * Answer: We don't know! What we know:
    * ~15% of the websites use a modern JavaScript framework (e.g. Vue or React) [Source: Web Almanac 2021](https://docs.google.com/spreadsheets/d/1zU9rHpI3nC6jTz3xgN6w13afW7x34xAKBh2IPH-lVxk/edit#gid=1851485826)
    * But not all are SPAs...
    
  * Not always a green field - not always SPAs - maybe LAMP, maybe Java based monoliths (traditional server-rendered)
  * Actually, most of the projects are "legacy"
    * jQuery/MooTools/...
  * Sometimes not migratable to SPAs (time/budget/domain knowledge in the code/experience of the team)
  * But still we want to add interactivity to such projects every now and then as well
    * With a modern approach!
    * Support devices with no JS as well

---

 Alpine.js - 0.1%

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
* createApp
* getters
* Methods (and compare to options api)
* mount to specific elements
* Lifecycle "hooks"
* `v-effect`
* Has a system for components
* Store via Vue's `reactive`
* Custom directive (optional)

### Limitations

* No `ref` nor `computed`
* No `render` functions (due to missing VDOM)
* SPA features like transitions, teleports, suspense and more
* Not treeshakable

### Live coding?

3. `petite-vue` vs. `alpine`?

* Inspired by alpine
* Both powered by VueJS reactivity
* petite-vue -> even more minimal, but "vue compatible" 
* Alpine -> steers towards own ecosystem

<!---

https://twitter.com/youyuxi/status/1410759893359874050

Vanilla.js 0 kB?

https://twitter.com/stauffermatt/status/1403798390585053190

-->