---
---

# Our Approach: Smart Network Design

<figure
    v-click
    class="absolute top-30 left-7 w-230"
    >
    <img src="/images/approach/network-optimization.png" />
    <figcaption class="text-center">AI-powered network optimization process</figcaption>
</figure>

<!--
Here's how our approach works. We start with a network of nodes connected by springs - like a molecular jungle gym. Our AI then optimizes two things: where the nodes are positioned and how strong each spring is. The magic happens when we use automatic differentiation - borrowed from machine learning - to optimize for both mechanical and acoustic properties simultaneously. This is like teaching the network to be both a shock absorber and a sound filter at the same time.
-->

---
hideInToc: true
---

# The Technical Innovation

<figure
    class="absolute top-50 left-7 w-230"
    >
    <img src="/images/approach/gradient-comparison.png" />
    <figcaption class="text-center">Traditional finite differences vs. automatic differentiation</figcaption>
</figure>

<!--
The technical breakthrough is in how we calculate gradients. Traditional methods use finite differences - imagine testing every single spring one at a time to see how it affects the outcome. That takes hours. We use automatic differentiation from JAX, which calculates all gradients simultaneously. It's like having thousands of parallel experiments running at once. This 100x speedup enables us to explore design spaces that were previously computationally impossible.
-->

---
hideInToc: true
---

# Dual Objective Optimization

<figure
    class="absolute top-40 left-12 w-220"
    >
    <img src="/images/approach/dual-optimization.png" />
    <figcaption class="text-center">Simultaneous optimization for Poisson's ratio and acoustic bandgaps</figcaption>
</figure>

<!--
The real challenge is optimizing for two very different properties simultaneously. We want a specific Poisson's ratio - how the material deforms - AND we want acoustic bandgaps - frequencies that can't propagate. It's like trying to design a car that's both fast and fuel-efficient. Our algorithm balances these competing objectives through a clever loss function that penalizes deviation from both targets. The AI learns to create structures that achieve both properties with minimal compromise.
-->

---
---

# Network Structure Analysis

<v-clicks>

- Initial configuration
  - 15×15 grid with controlled disorder
  - Average coordination: 5.48 (hexagonal-like)
  - Bond strengths: 0.5-3.0
- Optimization targets
  - Poisson's ratio: -0.5 to +0.5
  - Acoustic bandgaps: 1.5-2.5 (normalized frequency)
- Convergence criteria
  - Energy minimization
  - Gradient threshold: 10⁻¹⁰
  - Max iterations: 500

</v-clicks>

<!--
Let's look at the specifics. We start with a 15x15 grid of nodes - not too big to be computationally expensive, but large enough to show emergent properties. The slight disorder we introduce is crucial - it prevents the optimization from getting stuck in symmetric solutions. We can reliably achieve Poisson's ratios from -0.5 to +0.5, covering everything from extremely auxetic to conventional materials. The acoustic bandgaps we target are in the normalized frequency range of 1.5 to 2.5, which translates to useful frequencies for real applications.
-->
