### The challenge: non-natural materials with complex behavior

<figure
    v-click="1"
    v-motion
    :initial="{ opacity: 1 }"
    :click-4="{ opacity: 0 }"
    :leave="{ opacity: 0 }"
    class="absolute top-25 left-35 w-70 h-auto"
    >
    <img src="/images/intro/poisson.gif" rounded />
    <figcaption class="text-center text-sm">Normal material<sup>1</sup>, Poisson ratio > 0</figcaption>
</figure>

<figure
    v-click="2"
    v-motion
    :initial="{ opacity: 1, x: 0, y: 0 }"
    :click-4="{ x: 250, y: -140, opacity: 0.7 }"
    :click-5="{ opacity: 0 }"
    :leave="{ opacity: 1, x: 0, y: 0 }"
    class="absolute top-76 left-35 w-70 h-auto transition-all duration-500"
    >
    <img src="/images/intro/auxetic.gif" rounded/>
    <figcaption class="text-center text-sm">Auxetic material<sup>2</sup>, Poisson ratio < 0</figcaption>
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
    <img src="/images/intro/acoustic_structure.png" rounded/>
</figure>

<figure
    v-click="3"
    v-motion
    :initial="{ opacity: 1, x: 0, y: 0 }"
    :click-4="{ opacity: 0 }"
    :leave="{ opacity: 1 }"
    class="absolute top-76 right-50 w-55 h-auto transition-all duration-500"
    >
    <img src="/images/intro/acoustic_dos.png" rounded/>
    <figcaption class="text-center text-sm">Acoustic bandgap<sup>3</sup></figcaption>
</figure>

<Footnotes separator v-click="4">
  <Footnote :number=1><a href="https://makeagif.com/gif/auxetic-material-and-mechanism-design-bernhard-thomaszewski-ri_gDA">makeagif.com</a></Footnote>
  <Footnote :number=2><a href="https://makeagif.com/gif/understanding-poissons-ratio-iHVmOa">makeagif.com</a></Footnote>
  <Footnote :number=3><a href="https://www.nature.com/articles/s41598-020-73299-3">D'Alessandro, L. et al. Sci Rep 10, 16403 (2020) </a></Footnote>
</Footnotes>

<!--
Let's start with the fundamental problem we're solving. Most materials behave predictably – they get thinner when stretched, as shown in this normal material, and are characterized by having a positive Poisson ratio. But auxetic materials, shown here, do the opposite – they expand laterally when stretched, giving them a negative Poisson's ratio.
Separately, acoustic metamaterials can block specific sound frequencies through what we call bandgaps, shown in this figure. But combining these properties has been a major challenge –  That's the problem we set out to solve. But first, why would we even want to do this?
-->
