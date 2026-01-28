---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: ./assets/cover.jpeg
# some information about your slides (markdown enabled)
title: uMap Workshop
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# duration of the presentation
duration: 35min
dragPos:
  square: 709,292,136,162
---

# Web Mapping
## for Non-programmers

Using uMap

<br>

*Felipe Valdez*
<br>

*February 2026*

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
  Press Space for next page <carbon:arrow-right />
</div>

<img 
  src="./assets/Logo_uMap_01.png" 
  class="absolute"
  style="left: 675px; top: 300px; width: 250px; background-color: rgba(255, 255, 255, 0.7); padding: 10px; border-radius: 8px;"
  alt="uMap logo"
/>

<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
---

# Workshop contents

<br>

- 🤨 **What are Webmaps?** - WebMapping basics
- 💡 **Why use uMap?** - 
- 📺 **uMap interface** - code highlighting, live coding with autocompletion
- 🧑🏽‍💻 **Creating your first map** - embed Vue components to enhance your expressions
- 📍 **Creating data** - built-in recording and camera view
- 🎨 **Styling your map** - export to PDF, PPTX, PNGs, or even a hostable SPA
- 📲 **Importing / Exporting data** - virtually anything that's possible on a webpage is possible in Slidev
- 🌎 **Sharing your map** - virtually anything that's possible on a webpage is possible in Slidev

<br>
<br>


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, rgb(127, 58, 79) 10%, rgb(61, 36, 78) 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
Here is another comment.
-->

---
layout: two-cols
layoutClass: gap-16
transition: slide-up
---

# What is a Web Map?

A web map is an interactive map delivered over the internet through a web browser. Unlike static paper maps or simple images, web maps allow you to:

<br>
<br>

- 🔎 Zoom in and out
- ✋🏽 Pan across the map
- 🖱️ Click on features to see pop-ups
- ✅ Toggle layers on and off
- 👀 Search and navigate to specific places
- 🛜 Share and embed maps in websites, presentations, or social media

::right::

<div class="h-full flex items-center justify-center">
  <img src="./assets/map1.png" class="max-w-full max-h-100 object-contain" />
</div>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, rgb(127, 58, 79) 10%, rgb(61, 36, 78) 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
transition: slide-up
---

# Web Maps vs. Traditional Maps

Understanding the difference

| 📄 **Traditional Maps** | 🌐 **Web Maps** |
|:---|:---|
| Static, fixed scale | Interactive zoom levels |
| Limited information | Rich pop-ups with text, images, videos, links |
| Print or image file | Shareable links, embeddable in websites |
| Single view | Multiple layers you can control |
| One-way communication | Collaborative editing possible |

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, rgb(127, 58, 79) 10%, rgb(61, 36, 78) 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
layout: image-right
image: https://cover.sli.dev
---

# Code

Use code snippets and get the highlighting directly, and even types hover!

```ts [filename-example.ts] {all|4|6|6-7|9|all} twoslash
// TwoSlash enables TypeScript hover information
// and errors in markdown code blocks
// More at https://shiki.style/packages/twoslash
import { computed, ref } from 'vue'

const count = ref(0)
const doubled = computed(() => count.value * 2)

doubled.value = 2
```

<arrow v-click="[4, 5]" x1="350" y1="310" x2="195" y2="342" color="#953" width="2" arrowSize="1" />

<!-- This allow you to embed external code blocks -->
<<< @/snippets/external.ts#snippet

<!-- Footer -->

[Learn more](https://sli.dev/features/line-highlighting)

<!-- Inline style -->
<style>
.footnotes-sep {
  @apply mt-5 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style>

<!--
Notes can also sync with clicks

[click] This will be highlighted after the first click

[click] Highlighted with `count = ref(0)`

[click:3] Last click (skip two clicks)
-->


