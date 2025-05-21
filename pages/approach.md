---
---

### Our approach: Materials with dual functions

<div class="grid grid-cols-3 gap-8 mt-3">
  <div class="col-span-2 px-4 py-2 bg-blue-50 border-l-4 border-blue-500 rounded">
    <h4 class="text-lg font-bold">What are we optimizing?</h4>
    <div class="grid grid-cols-2 gap-3 mt-2">
      <div>
        <p class="font-bold">Mechanical: Poisson's ratio</p>
        <p class="text-sm">When stretched, most materials get thinner in transversal direction</p>
        <div class="text-xs mt-2">
          Common materials:
          <br>• Rubber: +0.5
          <br>• Steel: +0.3
          <br>• Cork: ≈0
          <br>• Auxetic: -0.1 to -1.0
        </div>
      </div>
      <div>
        <p class="font-bold">Acoustic: Bandgaps</p>
        <p class="text-sm">Specific frequencies can't pass through</p>
        <div class="text-xs mt-2">
          Like a filter that blocks:
          <br>• Traffic noise (50-1000 Hz)
          <br>• Machine vibrations
          <br>• But allows emergency sirens
        </div>
      </div>
    </div>
  </div>
  
  <div class="">
    <img src="/images/intro/network_app_1.png" class="w-70 h-auto mb-0" />
  </div>
</div>

$$\mathbf{F} = -\boxed{\color{red}{\nabla}}(E_{total} + \lambda_P P + \lambda_B B)$$


<div v-click class="mt-6 relative">
  
  <div class="absolute top-0 left-1/2 transform -translate-x-7 -translate-y-10">
    <div class="bg-yellow-100 text-red-600 font-semibold px-3 py-1 rounded-lg border border-red-400 shadow-md text-sm">
      The key challenge!
    </div>
  </div>
  
  <div class="text-center mt-4 text-sm">
    <p>Computing this gradient for thousands of parameters is computationally expensive</p>
    <p>Traditional methods use finite differences — slow and inaccurate</p>
  </div>
</div>


<!-- Footer with next slide indication -->
<div v-click class="absolute bottom-5 right-10 text-lg text-blue-500">
  ↓ How do we solve this?
</div>

<!--
These images show our network optimization approach in action. We start with a disordered network - a 15×15 grid of nodes connected by springs with slight random perturbations. This is our initial playground for optimization.

In the middle image, you can see our AI optimization in progress. The red arrows show how the nodes are moving as the algorithm searches for the optimal configuration. This is where JAX's automatic differentiation makes all the difference.

The right image shows the final optimized network. Notice how it's developed subtle structural changes that give it the special properties we're targeting. The gray ghost image shows where the network started, highlighting the significant transformation.

The key breakthrough is using automatic differentiation from JAX. Traditional methods test one spring at a time - imagine having to tweak thousands of parameters one by one. Our approach optimizes all parameters simultaneously, giving us a 100x speedup. That's the difference between waiting days for results versus getting them in minutes.
-->

---
---

### Our solution: network optimization with AI

<div class="grid grid-cols-3 gap-4 mt-2">
  <div v-click class="flex flex-col items-center">
    <img src="/images/intro/network_app_1.png" class="w-50 h-auto mb-0" />
    <figcaption class="text-center text-sm">1. Start with random network</figcaption>
  </div>
  
  <div v-click class="flex flex-col items-center">
    <img src="/images/intro/network_app_2.png" class="w-50 h-auto mb-0" />
    <figcaption class="text-center text-sm">2. Calculate gradients with JAX</figcaption>
  </div>
  
  <div v-click class="flex flex-col items-center">
    <img src="/images/intro/network_app_3.png" class="w-50 h-auto mb-0" />
    <figcaption class="text-center text-sm">3. Update network structure</figcaption>
  </div>
</div>

<div v-click class="mt-6 px-4 py-3 bg-blue-50 border-l-4 border-blue-500 rounded">
  <h4 class="text-lg font-bold">Key innovation: Automatic differentiation with JAX</h4>
</div>

<div v-after class="grid grid-cols-2 gap-4 mt-4">
  <div class="px-4 pt-2 pb-3 bg-red-50 border-l-4 border-red-500 rounded">
    <h5 class="text-md font-bold">Traditional method</h5>
    <p class="text-s">- Test one spring at a time ⏱️</p>
    <p class="text-s">- Hours of computation 🐢</p>
  </div>
  
  <div v-after class="px-4 pt-2 pb-3 bg-green-50 border-l-4 border-green-500 rounded">
    <h5 class="text-md font-bold">Our method</h5>
    <p class="text-s">- Calculate all gradients at once ⚡</p>
    <p class="text-s">- Minutes of computation 🚀</p>
  </div>
</div>

---
---

### Individual optimization of properties

<div grid="~ cols-2 gap-2" m="t-2">

  <h5 class="font-bold text-lg text-center">Auxetic</h5>

  <h5 class="font-bold text-lg text-center">Acoustic</h5>

  <div v-click grid="~ cols-2 gap-2" m="t--2">
  
  <img src="/images/results/auxetic.gif" class="w-100 h-auto mt-0" />

  <img src="/images/results/auxetic_curve.png" class="w-90 h-auto mt-4" />
  </div>

  <div v-click="3" grid="~ cols-2 gap-2" m="t--2">
  <img src="/images/results/acoustic_network.gif" class="w-100 h-auto mt-0" />

  <img src="/images/results/acoustic_dos.gif" class="w-100 h-auto mt-0" />  
  </div>

  <img v-click="2" src="/images/results/auxetic_comp.png" class="w-100 h-auto mb--2 ml-4" />

  <div v-click="4" grid="~ cols-2 gap-2" m="t-2">
  <img src="/images/results/acoustic_network.png" class="w-auto h-65% mt-4 ml-7" />

  <img src="/images/results/acoustic_compressed.png" class="w-95% h-auto mt-4" />
  </div>

</div>

<!--
The real magic happens when we optimize for both properties simultaneously. We want a specific Poisson's ratio - how the material deforms - AND acoustic bandgaps - frequencies that can't pass through. It's like designing a car that's both fast AND fuel-efficient. Our algorithm balances these competing objectives through a clever loss function that minimizes deviation from both targets.
-->

---
layout: center
---

1. Can we optimize for both properties simultaneously?

2. What are the benefits, if any, with auxetic networks on bandgap creation?