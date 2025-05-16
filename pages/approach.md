---
---

### Our approach: network optimization with AI

<div class="grid grid-cols-3 gap-4">
  <div v-click class="flex flex-col items-center">
    <img src="/images/intro/network_app_1.png" class="w-50 h-auto mb--2" />
    <figcaption class="text-center">initial network</figcaption>
  </div>
  
  <div v-click class="flex flex-col items-center">
    <img src="/images/intro/network_app_2.png" class="w-50 h-auto mb--2" />
    <figcaption class="text-center">calculate gradients</figcaption>
  </div>
  
  <div v-click class="flex flex-col items-center">
    <img src="/images/intro/network_app_3.png" class="w-50 h-auto mb--2" />
    <figcaption class="text-center">update network</figcaption>
  </div>
</div>

<div v-click class="mt-4 px-4 py-3 bg-blue-50 border-l-4 border-blue-500 rounded">
  <h4 class="text-lg font-bold">Key ingredient: automatic differentiation with JAX</h4>
</div>

<div v-click class="grid grid-cols-2 gap-4 mt-2">
  <div class="px-4 pt-2 pb-3 bg-red-50 border-l-4 border-red-500 rounded">
    <h5 class="text-lg font-bold -mt-1">Traditional method</h5>
    <p class="text-s">- test one spring at a time ⏱️</p>
    <p class="text-s">- hours of computation 🐢</p>
  </div>
  
  <div class="px-4 pt-2 pb-3 bg-green-50 border-l-4 border-green-500 rounded">
    <h5 class="text-lg font-bold -mt-1">Our method</h5>
    <p class="text-s">- calculate all gradients at once ⚡</p>
    <p class="text-s">- minutes of computation 🚀</p>
  </div>
</div>

<!--
These images show our network optimization approach in action. We start with a disordered network - a 15×15 grid of nodes connected by springs with slight random perturbations. This is our initial playground for optimization.

In the middle image, you can see our AI optimization in progress. The red arrows show how the nodes are moving as the algorithm searches for the optimal configuration. This is where JAX's automatic differentiation makes all the difference.

The right image shows the final optimized network. Notice how it's developed subtle structural changes that give it the special properties we're targeting. The gray ghost image shows where the network started, highlighting the significant transformation.

The key breakthrough is using automatic differentiation from JAX. Traditional methods test one spring at a time - imagine having to tweak thousands of parameters one by one. Our approach optimizes all parameters simultaneously, giving us a 100x speedup. That's the difference between waiting days for results versus getting them in minutes.
-->

---
---

# Dual Objective Optimization

<div class="grid grid-cols-2 gap-6">
  <div>
    <div v-click class="px-4 py-3 mb-4 bg-blue-50 border-l-4 border-blue-500 rounded">
      ### Poisson's Ratio (ν)
      
      > Controls how material deforms
      > 
      > Target: -0.5 to +0.5
    </div>
    
    <div v-click class="px-4 py-3 bg-purple-50 border-l-4 border-purple-500 rounded">
      ### Acoustic Bandgaps
      
      > Frequencies that can't propagate
      > 
      > Target: 1.5-2.5 (normalized)
    </div>
  </div>
  
  <div v-click class="flex flex-col items-center justify-center">
    <img src="/images/approach/dual-optimization.png" class="w-80 h-auto rounded shadow" />
    
    ### Challenge
    
    > Balancing competing objectives: mechanical and acoustic
  </div>
</div>

<div v-click class="mt-4 px-4 py-3 bg-yellow-50 border-l-4 border-yellow-500 rounded text-center">
  ## Our Innovation: Optimizing both properties without compromise
  
  **Like designing a car that's both fast AND fuel-efficient**
</div>

<!--
The real magic happens when we optimize for both properties simultaneously. We want a specific Poisson's ratio - how the material deforms - AND acoustic bandgaps - frequencies that can't pass through. It's like designing a car that's both fast AND fuel-efficient. Our algorithm balances these competing objectives through a clever loss function that minimizes deviation from both targets.
-->
