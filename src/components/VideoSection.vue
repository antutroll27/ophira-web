<template>
  <section class="w-full relative">
    <div class="w-full h-[500px] md:h-[750px] bg-gray-800 relative overflow-hidden group cursor-pointer">
      <!-- Placeholder for Video -->
      <img src="https://images.unsplash.com/photo-1497366216548-37526070297c?auto=format&fit=crop&q=80&w=2000" class="w-full h-full object-cover opacity-60 transition duration-500 group-hover:scale-105" alt="Video Background">
      <div class="absolute inset-0 flex items-center justify-center">
        <h2 class="text-6xl md:text-8xl font-black text-[#ccf32f] opacity-80 text-center leading-none select-none uppercase">
          Video File <br> Video File
        </h2>
      </div>
      <div class="absolute inset-0 flex items-center justify-center">
        <button class="w-20 h-20 bg-white rounded-full flex items-center justify-center shadow-lg hover:scale-110 transition">
          <i class="fa-solid fa-play text-2xl ml-1"></i>
        </button>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

