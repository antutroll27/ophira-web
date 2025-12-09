<template>
  <header class="relative bg-[#ccf32f] pt-28 pb-28 md:pt-32 md:pb-32 lg:pt-40 lg:pb-40 overflow-hidden">
    <div class="container mx-auto px-6 grid md:grid-cols-2 gap-12 items-center pt-10 pb-5">
      <div class="z-10">
        <h1 class="text-5xl md:text-7xl font-black leading-tight mb-6 text-black uppercase">
          Medium Length <br> Hero Goes Here
        </h1>
        <p class="text-lg mb-10 max-w-md font-light">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros dolor interdum nulla, ut commodo diam libero vitae erat.
        </p>
        <div class="flex space-x-4">
          <button class="bg-black text-white px-8 py-2 rounded-lg font-bold hover:bg-gray-800 transition shadow-lg">
            Get Started
          </button>
          <button class="bg-white text-black px-8 py-2 rounded-lg font-bold hover:bg-gray-100 transition shadow-lg">
            Learn More
          </button>
        </div>
      </div>
      
      <!-- Phone Mockup -->
      <div class="relative flex justify-center z-10">
        <img
          :src="mockup"
          alt="Product mockup"
          class="w-full max-w-xs md:max-w-sm lg:max-w-md drop-shadow-2xl"
        />
      </div>
    </div>
  </header>
</template>

<script setup>
import mockup from '../assets/Mockup.png'
</script>

