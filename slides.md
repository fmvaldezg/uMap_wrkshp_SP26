---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /assets/cover.jpeg
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
  src="/assets/Logo_uMap_01.png" 
  class="absolute"
  style="left: 675px; top: 300px; width: 250px; background-color: rgba(255, 255, 255, 0.7); padding: 10px; border-radius: 8px;"
  alt="uMap logo"
/>

<div class="abs-br m-6 text-xl">
  <a href="https://charlesstudy.temple.edu/calendar/workshops?&t=g&d=0000-00-00&cal%5B%5D=6197&ct%5B%5D=69157" title="More Workshops" target="_blank" class="slidev-icon-btn">
    <carbon:information />
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
- 💡 **Why use uMap?** - uMap features
- 📺 **uMap interface** - view vs. edit mode
- 🧑🏽‍💻 **Creating your first map** - Adding a title, description and layout.
- 📍 **Creating data** - Adding points, lines or poligons. Adding features.
- 🎨 **Styling your map** - Changing icons, colors and stiles. 
- 📲 **Importing / Exporting data** - import a file or a url. 
- 🌎 **Sharing your map** - sharing a link, embeding the map or printing.

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
  <img src="/assets/map1.png" class="max-w-full max-h-100 object-contain" />
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
image: /assets/umap_web.png
backgroundSize: contain
---

# Why use uMap?

1. **Free and Open Source** - no licensing costs
2. **Quick and Easy** - build maps without coding skills  
3. **Privacy Focused** - anonymous creation, no personal data required
4. **Collaborative** - high interoperability
5. **Rich Customization** - markers, polygons, heatmaps, storytelling
6. **Easy Embedding** - works on any website
7. **Built on OpenStreetMap** - open geographic data

<!-- Footer -->
[Learn more](https://umap-project.org/)

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
layout: section
---

# [Hands on](https://umap.openstreetmap.fr/en/map/anonymous-edit/1351201:bpyjlr8apj2HygdyNpFlK5CpZbJZknjfejkwACH3CFQ)

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
layout: default
--- 

<iframe style="width: 100%; height: 450px; border: 0;" allowfullscreen allow="geolocation" src="//umap.openstreetmap.fr/en/map/a-map-of-philadelphia_1351615?scaleControl=false&miniMap=false&scrollWheelZoom=false&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=null&captionBar=false&captionMenus=false"></iframe><p><a href="//umap.openstreetmap.fr/en/map/a-map-of-philadelphia_1351615?scaleControl=false&miniMap=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=caption&captionBar=false&captionMenus=true">See full screen</a></p>


--- 
layout: image
image: /assets/view_mode.png
backgroundSize: contain
--- 

# View Mode

<style>
h1 {
  background-color: rgba(248, 248, 248, 0.7);
  padding: 1rem 2rem;
  border-radius: 8px;
  text-align: center;
  position: absolute;
  bottom: 2rem;
  right: 6rem;
  margin: 0;
  max-width: fit-content;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  color: #333333;
}
</style>

--- 
layout: image
image: /assets/edit_mode.png
backgroundSize: contain
--- 

# Edit Mode

<style>
h1 {
  background-color: rgba(248, 248, 248, 0.7);
  padding: 1rem 2rem;
  border-radius: 8px;
  text-align: center;
  position: absolute;
  bottom: 2rem;
  right: 6rem;
  margin: 0;
  max-width: fit-content;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  color: #333333;
}
</style>

--- 
layout: image-right
image: /assets/first.gif
backgroundSize: contain
--- 

# Creating your first map

1. Head to [https://umap-project.org/](https://umap-project.org/)
2. Click on 'Create a map'
3. Choose an instance (FR recommended)
4. Start editing your map

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
layout: image
transition: slide-up
image: /assets/workshoppromo.png
--- 

--- 
layout: end
---

Contact us at:\
felipe.valdez@temple.edu \
<br>
Visit our guides:\
https://guides.temple.edu/gis-mapping

<style>
.slidev-layout.end {
  background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);
}
</style>