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
Our approach tackles two key properties. Mechanically, we optimize the Poisson's ratio – how materials deform when stretched. Acoustically, we create bandgaps that block specific sound frequencies.

The real challenge lies in this equation. See the gradient operator highlighted in red? Computing this gradient for thousands of parameters is incredibly expensive using traditional methods like finite differences – it's slow and inaccurate.

Our solution leverages automatic differentiation with JAX, which efficiently computes exact gradients for all parameters simultaneously. This makes the previously impossible task of dual optimization feasible.
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

<!--
Here's how we implement our solution. We start with a random network of nodes connected by springs. Then, using JAX, we calculate gradients for thousands of parameters simultaneously, efficiently updating the network structure.

The key innovation is automatic differentiation. Traditional methods test one spring at a time, taking hours of computation. Our method calculates all gradients at once, completing in minutes what used to take days. This 100x speedup makes dual property optimization practical for the first time.
-->

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
Before tackling dual optimization, we verified we could optimize each property individually.
On the left, you see our auxetic optimization. We can reliably design networks with Poisson ratios ranging from -0.5 to 0.5. The key structural feature for auxetic behavior is the prevalence of sharp angles, particularly around 30 degrees.

On the right is our acoustic optimization. We successfully created networks with bandgaps at specific target frequencies. When compressed, these networks show a significant reduction in vibrational states within the target frequency range.
-->

---
layout: center
---

1. Can we optimize for both properties simultaneously?

2. What are the benefits, if any, with auxetic networks on bandgap creation?