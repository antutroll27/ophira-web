<template>
  <section class="py-24 bg-white/50">
    <div class="container mx-auto px-6">
      <div class="max-w-2xl mb-16">
        <h2 class="text-4xl font-black mb-6">Medium length heading about features of the app</h2>
        <p class="text-gray-600 mb-8">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.
        </p>
        <button class="bg-[#ccf32f] text-black px-8 py-3 rounded-full font-bold hover:bg-opacity-80 transition shadow-md">
          View all features
        </button>
      </div>
      <div class="grid md:grid-cols-4 gap-8">
        <div v-for="(feature, index) in features" :key="index" class="bg-[#ccf32f]/10 p-8 rounded-2xl hover:bg-[#ccf32f]/20 transition duration-300">
          <div class="w-12 h-12 bg-black text-white rounded-xl flex items-center justify-center mb-6 text-xl">
            <i :class="feature.icon"></i>
          </div>
          <h3 class="text-xl font-bold mb-3">{{ feature.title }}</h3>
          <p class="text-sm text-gray-600 leading-relaxed">{{ feature.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const features = [
  { title: "Real-time Sync", icon: "fa-arrows-rotate", description: "Seamlessly sync data across all your devices in real-time without lags." },
  { title: "Secure Encryption", icon: "fa-shield-halved", description: "Bank-grade encryption ensures your data stays private and secure." },
  { title: "Smart Analytics", icon: "fa-chart-pie", description: "Gain insights into your usage patterns with detailed visual reports." },
  { title: "Global Access", icon: "fa-globe", description: "Access your dashboard from anywhere in the world with 99.9% uptime." }
]
</script>

