---
---

### the challenge: materials with complex behavior

<figure
    v-click
    class="absolute top-25 left-35 w-70 h-auto"
    >
    <img src="/images/intro/poisson.gif" />
    <figcaption class="text-center">Normal material<sup>1</sup></figcaption>
</figure>

<figure
    v-click
    class="absolute top-76 left-35 w-70 h-auto"
    >
    <img src="/images/intro/auxetic.gif" />
    <figcaption class="text-center">Auxetic material<sup>2</sup></figcaption>
</figure>

<figure
    v-click
    class="absolute top-25 right-50 w-50 h-auto"
    >
    <img src="/images/intro/acoustic.png"/>
    <figcaption class="text-center">Acoustic bandgap<sup>3</sup></figcaption>
</figure>

<Footnotes separator v-click=3>
  <Footnote :number=1><a href="https://makeagif.com/gif/auxetic-material-and-mechanism-design-bernhard-thomaszewski-ri_gDA">makeagif.com</a></Footnote>
  <Footnote :number=2><a href="https://makeagif.com/gif/understanding-poissons-ratio-iHVmOa">makeagif.com</a></Footnote>
  <Footnote :number=3><a href="https://www.nature.com/articles/s41598-020-73299-3">D’Alessandro, L. et al. Sci Rep 10, 16403 (2020) </a></Footnote>
</Footnotes>

<!--
Let's start with a simple question: what if materials could do the impossible? Most materials, when you squeeze them, bulge out to the sides - like squeezing a stress ball. But what if we could design materials that actually get thinner when compressed? These are called auxetic materials. And what if these same materials could also block specific sound frequencies? This combination has never been achieved before.
-->

---
hideInToc: true
---

# Why This Matters: Real Impact

<figure
    v-click
    class="absolute top-30 left-60 w-40 h-40"
    >
    <img src="/images/applications/medical-stent.png" />
    <figcaption class="text-center">Smart medical stents<sup>1</sup></figcaption>
</figure>

<figure
    v-after
    class="absolute top-90 left-60 w-40 h-40"
    >
    <img src="/images/applications/earthquake-building.png" />
    <figcaption class="text-center">Earthquake-resistant buildings<sup>2</sup></figcaption>
</figure>

<Footnotes separator v-after>
  <Footnote :number=1>Stents that expand appropriately when deployed</Footnote>
  <Footnote :number=2>Buildings that adapt to seismic waves</Footnote>
</Footnotes>

<figure
    v-click
    class="absolute top-30 left-130 w-40 h-40"
    >
    <img src="/images/applications/aerospace.png" />
    <figcaption class="text-center">Aerospace vibration control<sup>3</sup></figcaption>
</figure>

<figure
    v-after
    class="absolute top-90 left-130 w-40 h-40"
    >
    <img src="/images/applications/market-size.png" />
    <figcaption class="text-center">$50B+ market by 2030<sup>4</sup></figcaption>
</figure>

<Footnotes separator v-after>
  <Footnote :number=3>Lightweight materials for spacecraft and aircraft</Footnote>
  <Footnote :number=4>Metamaterials market projection</Footnote>
</Footnotes>

<!--
Why should you care about these impossible materials? Well, imagine medical stents that expand perfectly when inserted into blood vessels, or buildings that can adapt their structure during earthquakes to protect occupants. These materials could revolutionize aerospace by creating lightweight structures that block engine vibrations. The metamaterials market is projected to exceed $50 billion by 2030, and our work opens entirely new possibilities in this space.
-->

---
hideInToc: true
preload: false
---

# The Physics Behind It

<figure
    v-click
    class="absolute top-30 left-50 w-142"
    >
    <img src="/images/physics/poisson-ratio-demo.gif" />
    <figcaption class="text-center">Poisson's ratio in action<sup>1</sup></figcaption>
</figure>

<div
    v-click
    class="absolute top-75 left-20 right-20"
    >
    
| Material Type | Poisson's Ratio | Behavior |
| ------------- | --------------- | -------- |
| Rubber        | ~0.5            | Maximum lateral expansion |
| Steel         | ~0.3            | Moderate lateral expansion |
| Cork          | ~0              | No lateral change |
| **Auxetic**   | **< 0**         | **Lateral contraction!** |

</div>

<Footnotes separator v-after>
  <Footnote :number=1>Visual demonstration of different Poisson's ratios</Footnote>
</Footnotes>

<!--
Let me quickly explain the physics. Poisson's ratio describes how materials deform. When you stretch rubber, it gets thinner - that's a positive Poisson's ratio. Cork barely changes width when stretched - that's near zero. But auxetic materials? They get wider when stretched, defying our intuition. This property, combined with acoustic bandgaps that block specific sound frequencies, creates unprecedented opportunities for material design.
-->

---
layout: center
class: text-center
---

# Our Innovation: AI + Materials Science

<div
    v-click
    class="text-2xl my-8"
    >
    Networks of Springs + AI Optimization = <span v-mark.circle.orange>Impossible Materials</span>
</div>

<v-clicks>

<br>

## Key Breakthrough

- 100x faster than traditional methods
- Simultaneous optimization of multiple properties  
- Works with disordered (non-perfect) structures

</v-clicks>

<!--
Our key innovation combines network structures - think of nodes connected by springs - with cutting-edge AI optimization. Using automatic differentiation from machine learning, we can optimize these networks 100 times faster than traditional methods. This speed allows us to simultaneously design for multiple properties that were previously thought incompatible. And unlike previous approaches that required perfect periodic structures, our method works with disordered networks, making it more practical for real-world manufacturing.
-->
