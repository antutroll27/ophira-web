<template>
  <nav class="fixed w-full z-50 transition-all duration-300" :class="isScrolled ? 'bg-white/90 backdrop-blur-md shadow-sm py-3' : 'bg-transparent py-5'">
    <div class="container mx-auto px-6 flex justify-between items-center">
      <!-- Logo -->
      <img :src="logoImage" alt="Ophira" class="h-12 md:h-14 w-auto mt-3 md:mt-4">
      <!-- Desktop Menu -->
      <div class="hidden md:flex items-center space-x-10 lg:space-x-16 pt-6 md:pt-7 pb-2">
        <a href="#howitworks" class="text-lg font-normal hover:text-gray-600 transition">How it works</a>
        <a href="#benefits" class="text-lg font-normal hover:text-gray-600 transition">Benefits</a>
        <a href="#pricing" class="text-lg font-normal hover:text-gray-600 transition">Pricing</a>
        <a href="#faqs" class="text-lg font-normal hover:text-gray-600 transition">FAQs</a>
        <button class="bg-black text-[#ccf32f] px-5 py-2 rounded-md text-sm font-semibold hover:bg-gray-800 transition">
          Get Started
        </button>
      </div>
      <!-- Mobile Menu Button -->
      <button @click="$emit('toggle-mobile-menu')" class="md:hidden text-2xl">
        <i class="fa-solid fa-bars"></i>
      </button>
    </div>
  </nav>
</template>

<script setup>
import logoImage from '../assets/solutions.svg'

defineProps({
  isScrolled: {
    type: Boolean,
    default: false
  }
})

defineEmits(['toggle-mobile-menu'])
</script>

