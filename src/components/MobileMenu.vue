<template>
  <div v-if="isOpen" class="fixed inset-0 bg-white z-40 flex flex-col items-center justify-center space-y-8 md:hidden">
    <button @click="$emit('close')" class="absolute top-6 right-6 text-2xl">
      <i class="fa-solid fa-xmark"></i>
    </button>
    <a href="#nft" @click="$emit('close')" class="text-2xl font-bold">NFT</a>
    <a href="#about" @click="$emit('close')" class="text-2xl font-bold">About</a>
    <a href="#pricing" @click="$emit('close')" class="text-2xl font-bold">Pricing</a>
    <a href="#faq" @click="$emit('close')" class="text-2xl font-bold">FAQ</a>
  </div>
</template>

<script setup>
defineProps({
  isOpen: {
    type: Boolean,
    default: false
  }
})

defineEmits(['close'])
</script>

