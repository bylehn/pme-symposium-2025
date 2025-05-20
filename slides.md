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
layout: table-of-contents
hideInToc: true
---

<!--
Here's what we'll cover in the next 12 minutes. Let's start with understanding what makes these materials special.
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
layout: center
class: text-center
---

# Acknowledgments

<div bg="blue-50" p="4" rounded shadow m="b-6 t-4">
  <h3 text="blue-800" m="b-2">Co-Authors</h3>
  
  <div m="b-2">
    <span text="lg font-bold">Abhishek K. Sharma, PhD</span> • 
    <span text="lg font-bold">Cesar A. Castro Rubio</span> • 
    <span text="lg font-bold">Juan J. de Pablo, PhD</span>
  </div>
  
  <div text="gray-600 sm">Cooper Union • University of Chicago • New York University</div>
</div>

<div bg="green-50" p="4" rounded shadow m="b-6">
  <h3 text="green-800" m="b-2">Research Support</h3>
  
  <div>Pritzker School of Molecular Engineering • De Pablo Research Group</div>
  <div text="gray-600 sm" m="t-2">This work was supported by NSF grant #XXXX</div>
</div>

<div m="t-6">
  <h2 text="2xl" m="b-4">Thank You!</h2>
  
  <div flex="~ gap-4" justify="center">
    <a href="https://github.com/bylehn/saxophone" bg="blue-50" p="2" rounded hover:bg="blue-100">
      <carbon:logo-github class="text-xl mr-1 inline" /> bylehn/saxophone
    </a>
    
    <a href="mailto:fbylehn@uchicago.edu" bg="green-50" p="2" rounded hover:bg="green-100">
      <carbon:email class="text-xl mr-1 inline" /> fbylehn@uchicago.edu
    </a>
  </div>
</div>

<!--
I want to thank my co-authors for their invaluable contributions to this work. Abhishek brought expertise in materials optimization, Cesar helped develop the computational framework, and Professor de Pablo provided guidance throughout the project.

I'm also grateful to the entire De Pablo research group and the Pritzker School of Molecular Engineering for supporting this research.

Thank you for your attention! I'm happy to answer any questions.
-->