<template>
  <nav class="fixed w-full z-50 transition-all duration-300" :class="isScrolled ? 'bg-white/90 backdrop-blur-md shadow-sm py-3' : 'bg-transparent py-5'">
    <div class="container mx-auto px-6 flex justify-between items-center">
      <!-- Logo -->
      <img :src="logoImage" alt="Ophira" class="h-8 w-auto">
      <!-- Desktop Menu -->
      <div class="hidden md:flex items-center space-x-12 pt-5 pb-5">
        <a href="#howitworks" class="text-lg font-medium hover:text-gray-600 transition">How it works</a>
        <a href="#benefits" class="text-lg font-medium hover:text-gray-600 transition">Benefits</a>
        <a href="#pricing" class="text-lg font-medium hover:text-gray-600 transition">Pricing</a>
        <a href="#faqs" class="text-lg font-medium hover:text-gray-600 transition">FAQs</a>
        <button class="bg-black text-white px-5 py-2 rounded-sm text-sm font-semibold hover:bg-gray-800 transition">
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
import logoImage from '../assets/ophiralogo.png'

defineProps({
  isScrolled: {
    type: Boolean,
    default: false
  }
})

defineEmits(['toggle-mobile-menu'])
</script>

