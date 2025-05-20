---
theme: academic
layout: cover
class: text-white
transition: fade
fonts:
  sans: Plus Jakarta Sans
  serif: Robot Slab
  mono: Fira Code
hideInToc: true
coverAuthor1: Fabian Byléhn
coverAuthor2: Abhishek K. Sharma  
coverAuthor3: Cesar A. Castro Rubio
coverAuthor4: Juan J. de Pablo
coverAuthorUrl1: https://pme.uchicago.edu/
coverAuthorUrl2: https://cooper.edu/
coverAuthorUrl3: https://pme.uchicago.edu/
coverAuthorUrl4: https://pme.uchicago.edu/
coverBackgroundUrl: /images/cover_v2.png
coverBackgroundSource: Background image created with ChatGPT
coverBackgroundSourceUrl: https://chatgpt.com
coverDate: May 22, 2025
themeConfig:
  paginationX: r
  paginationY: t
  paginationPagesDisabled: [1]
title: Designing Materials That Break Physics Rules
info: |
  ## Inverse Design of Multifunctional Networks through Differentiable Optimization
  
  Smart materials with dual superpowers: negative Poisson's ratio and acoustic bandgaps
  
  - [Code](https://github.com/bylehn/saxophone)
  - [Contact](mailto:fbylehn@uchicago.edu)
---

<h2 style="max-width: 70%">When Materials Break the Rules:</h2>
Engineering Networks That Control Both Shape and Sound

<div class="absolute bottom-25 left-14 right-0 text-left">
  <p class="text-l">
    <a href="https://pme.uchicago.edu/" class="text-white hover:underline">Fabian Byléhn</a><sup>1</sup>, 
    <a href="https://cooper.edu/" class="text-white opacity-50 hover:underline">Abhishek K. Sharma</a><sup>2</sup>, 
    <a href="https://pme.uchicago.edu/" class="text-white opacity-50 hover:underline">Cesar A. Castro Rubio</a><sup>1</sup>, 
    <a href="https://pme.uchicago.edu/" class="text-white opacity-50 hover:underline">Juan J. de Pablo</a><sup>1,3</sup>
  </p>
  <p class="text-sm mt-2 opacity-80">
    <sup>1</sup>University of Chicago, <sup>2</sup>Cooper Union, <sup>3</sup>New York University
  </p>
</div>

<div class="abs-tl ml-0 my--20 flex gap-2 scale-75 origin-top-left">
  <a href="https://pme.uchicago.edu/" target="_blank" alt="PME"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <img src="/images/pme_logo_white.png" class="w-80 h-auto" />
  </a>
</div>

<div class="abs-tr mx-26 my-6 flex gap-2">
  <a href="https://github.com/bylehn/saxophone" target="_blank" alt="GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<div class="abs-tr mx-16 my-6 flex gap-2">
  <a href="/slides-export.pdf" target="_blank" alt="Slides"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-presentation-file />
  </a>
</div>

<div class="abs-tr m-6 flex gap-2">
  <a href="mailto:bylehn@uchicago.edu" target="_blank" alt="Contact"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-email />
  </a>
</div>

<!--
Good morning everyone! I'm Fabian Byléhn, a PhD candidate at PME. Today I'm excited to share how we're using AI to design materials that literally break the rules of physics.
-->

---
src: ./pages/challenge.md
---

---
src: ./pages/applications.md
---

---
src: ./pages/approach.md
---

---
src: ./pages/results.md
---

---
src: ./pages/conclusions.md
---

---
hideInToc: true
---

### Acknowledgments

<div grid="~ cols-2 gap-2" m="t-2">

  <div float="center" w="100%" h="100%" bg="blue-50" p="4" rounded-lg shadow m="r-4">
    <h5 text="blue-800 xl" m="b-2">Co-Authors</h5>
    <p m="b-1"><span text="lg font-bold">Abhishek Sharma, PhD</span> <span text="gray-600 sm">(Cooper Union)</span></p>
    <p m="b-1"><span text="lg font-bold">Cesar Castro Rubio</span> <span text="gray-600 sm">(UChicago)</span></p>
    <p><span text="lg font-bold">Prof. Juan de Pablo </span> <span text="gray-600 sm">(UChicago & NYU)</span></p>
  </div>

  <div float="right" w="100%" h="100%" bg="green-50" p="4" rounded-lg shadow>
    <h5 text="green-800 xl" m="b-2">SaXoPhone Package</h5>
    <p m="b-2" text="lg">
      <span font="bold">S</span>imulation of 
      <span font="bold">A</span>u<span font="bold">X</span>etics and 
      Ph<span font="bold">O</span>no<span font="bold">N</span>ics 
    </p>
    <p><carbon:code class="inline" /> Open-source Python with JAX</p>
    <p text="left" m="t-4">
      <a href="https://github.com/bylehn/saxophone" bg="white" p="2" rounded shadow>
        <carbon:logo-github class="text-xl mr-1 inline" /> github.com/bylehn/saxophone
      </a>
    </p>
  </div>
</div>

<div grid="~ cols-1 gap-2" m="t-2" text-center>
  <img src="/images/group-photo.png" h="50" ml-70 rounded shadow />
  <p text="sm gray-600">de Pablo Research Group, University of Chicago</p>
</div>

<!--
I'd like to thank my co-authors for their invaluable contributions. Abhishek brought expertise in materials optimization, Cesar helped develop the computational framework, and Professor de Pablo provided guidance throughout the project.

I'm excited to announce our open-source Python package called SaXoPhone - the Simulation of Auxetics and Phonics Engine. The name highlights our dual focus on auxetic materials and acoustic properties. Built on JAX for differentiable optimization, it's 100x faster than traditional approaches.

I'm also grateful to the entire De Pablo research group shown in the photo. Their support and collaboration were essential to this project's success.

Thank you for your attention! I'm happy to answer any questions.
-->