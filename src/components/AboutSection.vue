<template>
  <section id="about" class="py-24 bg-[#ccf32f] overflow-hidden">
    <div class="container mx-auto px-6 grid md:grid-cols-2 gap-16 items-center">
      <div>
        <span class="font-bold text-sm uppercase tracking-wider mb-2 block">About us</span>
        <h2 class="text-4xl md:text-5xl font-black mb-6">How we started</h2>
        <p class="mb-6 font-medium">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros dolor interdum nulla.
        </p>
        <p class="mb-6 font-medium">
          Mauris sed nisi sed libero commodo placerat. In pulvinar nibh ipsum, sit amet hendrerit odio pharetra et.
        </p>
      </div>
      
      <!-- Image Collage -->
      <div class="relative h-[400px] w-full">
        <!-- Image 1 -->
        <div class="absolute top-0 right-0 w-48 h-64 bg-gray-900 rounded-lg overflow-hidden shadow-2xl transform rotate-3 z-10 border-4 border-white">
          <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?auto=format&fit=crop&q=80&w=600" class="w-full h-full object-cover">
        </div>
        <!-- Image 2 -->
        <div class="absolute top-20 right-24 w-48 h-64 bg-gray-800 rounded-lg overflow-hidden shadow-2xl transform -rotate-6 z-20 border-4 border-white">
          <img src="https://images.unsplash.com/photo-1542744173-8e7e53415bb0?auto=format&fit=crop&q=80&w=600" class="w-full h-full object-cover">
        </div>
        <!-- Image 3 -->
        <div class="absolute top-40 right-48 w-48 h-64 bg-gray-700 rounded-lg overflow-hidden shadow-2xl transform rotate-6 z-30 border-4 border-white">
          <img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?auto=format&fit=crop&q=80&w=600" class="w-full h-full object-cover">
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

