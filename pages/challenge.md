---
---

### The challenge: materials with complex behavior

<figure
    v-click="1"
    v-motion
    :initial="{ opacity: 1 }"
    :click-4="{ opacity: 0 }"
    :leave="{ opacity: 1 }"
    class="absolute top-25 left-35 w-70 h-auto"
    >
    <img src="/images/intro/poisson.gif" rounded />
    <figcaption class="text-center">Normal material<sup>1</sup></figcaption>
</figure>

<figure
    v-click="2"
    v-motion
    :initial="{ opacity: 1, x: 0, y: 0 }"
    :click-4="{ x: 200, y: -150, opacity: 0.7 }"
    :click-5="{ opacity: 0 }"
    :leave="{ opacity: 1, x: 0, y: 0 }"
    class="absolute top-76 left-35 w-70 h-auto transition-all duration-500"
    >
    <img src="/images/intro/auxetic.gif" rounded/>
    <figcaption class="text-center">Auxetic material<sup>2</sup></figcaption>
</figure>

<figure
    v-click="3"
    v-motion
    :initial="{ opacity: 1, x: 0, y: 0 }"
    :click-4="{ x: -150, y: 60, opacity: 0.7 }"
    :click-5="{ opacity: 0 }"
    :leave="{ opacity: 1, x: 0, y: 0 }"
    class="absolute top-25 right-50 w-50 h-auto transition-all duration-500"
    >
    <img src="/images/intro/acoustic.png" rounded/>
    <figcaption class="text-center">Acoustic bandgap<sup>3</sup></figcaption>
</figure>

<!-- Question mark that appears after the images meet -->
<div
    v-click="5"
    v-motion
    :initial="{ opacity: 0, scale: 0.5 }"
    :enter="{ opacity: 1, scale: 2.5 }"
    :leave="{ opacity: 0 }"
    class="absolute top-45 left-[48%] text-8xl font-bold text-black-500"
    >
    ?
</div>

<Footnotes separator v-click="3">
  <Footnote :number=1><a href="https://makeagif.com/gif/auxetic-material-and-mechanism-design-bernhard-thomaszewski-ri_gDA">makeagif.com</a></Footnote>
  <Footnote :number=2><a href="https://makeagif.com/gif/understanding-poissons-ratio-iHVmOa">makeagif.com</a></Footnote>
  <Footnote :number=3><a href="https://www.nature.com/articles/s41598-020-73299-3">D'Alessandro, L. et al. Sci Rep 10, 16403 (2020) </a></Footnote>
</Footnotes>