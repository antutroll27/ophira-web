<template>
  <header class="relative bg-[#ccf32f] pt-40 pb-40 overflow-hidden">
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
        <div class="relative w-72 h-[580px] bg-black rounded-[3rem] border-8 border-black shadow-2xl overflow-hidden">
          <!-- Screen Content Mock -->
          <div class="w-full h-full bg-gray-900 flex flex-col items-center pt-8 px-4">
            <div class="w-full flex justify-between text-gray-400 text-xs mb-4">
              <span>9:41</span>
              <div class="flex space-x-1">
                <i class="fa-solid fa-signal"></i>
                <i class="fa-solid fa-wifi"></i>
                <i class="fa-solid fa-battery-full"></i>
              </div>
            </div>
            <!-- Mock App UI -->
            <div class="w-full bg-gray-800 h-32 rounded-xl mb-4 p-4">
              <div class="h-2 w-12 bg-gray-600 rounded mb-2"></div>
              <div class="h-8 w-24 bg-[#ccf32f] rounded"></div>
            </div>
            <div class="grid grid-cols-2 gap-3 w-full">
              <div class="bg-gray-800 h-24 rounded-xl flex items-center justify-center border border-[#ccf32f]/30">
                <i class="fa-solid fa-bolt text-[#ccf32f] text-xl"></i>
              </div>
              <div class="bg-gray-800 h-24 rounded-xl flex items-center justify-center">
                <i class="fa-solid fa-chart-line text-gray-500 text-xl"></i>
              </div>
              <div class="bg-gray-800 h-24 rounded-xl flex items-center justify-center">
                <i class="fa-solid fa-wallet text-gray-500 text-xl"></i>
              </div>
              <div class="bg-gray-800 h-24 rounded-xl flex items-center justify-center">
                <i class="fa-solid fa-gear text-gray-500 text-xl"></i>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
</script>

