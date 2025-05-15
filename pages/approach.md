---
---

# Our Approach: Network Optimization with AI

<figure
    v-click
    class="absolute top-28 left-4 w-115"
    >
    <img src="/images/approach/network-optimization.png" />
    <figcaption class="text-center">AI-powered network optimization process</figcaption>
</figure>

<div v-after class="absolute top-35 right-4 w-110">
  <h3 class="text-xl mb-4 font-bold">Key Innovation: JAX + Automatic Differentiation</h3>
  
  <div class="grid grid-cols-2 gap-4">
    <div class="bg-red-50 p-4 rounded">
      <p class="font-semibold">Traditional</p>
      <p class="text-sm">Finite differences</p>
      <p class="text-xs text-gray-600">Hours per optimization</p>
    </div>
    
    <div class="bg-green-50 p-4 rounded">
      <p class="font-semibold">Our Method</p>
      <p class="text-sm">Automatic differentiation</p>
      <p class="text-xs text-gray-600">Minutes per optimization</p>
    </div>
  </div>
  
  <h3 class="mt-4 font-bold text-3xl text-center text-green-600">100x Speedup!</h3>
</div>

<!--
Our approach is elegantly simple yet powerful. We model materials as networks of nodes connected by springs. Then we use AI to optimize two things: node positions and spring strengths. The breakthrough is using automatic differentiation from JAX - borrowed from machine learning. Instead of testing each spring one at a time, we calculate all gradients simultaneously. This gives us a 100x speedup, enabling optimization that was previously impossible.
-->

---
---

# Dual Objective Optimization

<div class="grid grid-cols-2 gap-8 h-full items-center">
  <div>
    <h3 class="text-xl font-bold mb-4">What We Optimize</h3>
    
    <v-clicks>
    
    <div class="mb-6">
      <h4 class="font-semibold text-lg text-blue-600">Poisson's Ratio (ν)</h4>
      <p>How material deforms under stress</p>
      <p class="text-sm text-gray-600">Target: -0.5 to +0.5</p>
    </div>
    
    <div>
      <h4 class="font-semibold text-lg text-purple-600">Acoustic Bandgaps</h4>
      <p>Frequencies that can't propagate</p>
      <p class="text-sm text-gray-600">Target: 1.5-2.5 (normalized)</p>
    </div>
    
    </v-clicks>
  </div>
  
  <div v-click>
    <img src="/images/approach/dual-optimization.png" class="rounded-lg shadow-lg" />
    <p class="text-center mt-2 text-sm">Balancing competing objectives simultaneously</p>
  </div>
</div>

<div v-click class="absolute bottom-8 left-0 right-0 text-center">
  <p class="text-xl font-bold">Challenge: Optimizing both properties without compromising either</p>
</div>

<!--
The real magic happens when we optimize for both properties simultaneously. We want a specific Poisson's ratio - how the material deforms - AND acoustic bandgaps - frequencies that can't pass through. It's like designing a car that's both fast AND fuel-efficient. Our algorithm balances these competing objectives through a clever loss function that minimizes deviation from both targets.
-->
