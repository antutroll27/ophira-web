<template>
  <section id="pricing" class="py-24 bg-white">
    <div class="container mx-auto px-6">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="bg-[#ccf32f] px-3 py-1 rounded-full text-xs font-bold uppercase tracking-widest mb-4 inline-block">Pricing</span>
        <h2 class="text-4xl font-black mb-4">Simple, Scalable Pricing</h2>
        <p class="text-gray-600 mb-8">Simple, transparent pricing that grows with you. Try any plan free for 30 days.</p>
        
        <!-- Toggle -->
        <div class="flex items-center justify-center space-x-4">
          <span class="text-sm font-bold" :class="!isAnnual ? 'text-black' : 'text-gray-400'">Monthly</span>
          <button @click="isAnnual = !isAnnual" class="w-16 h-8 bg-gray-200 rounded-full relative transition-colors duration-300">
            <div class="absolute top-1 left-1 w-6 h-6 bg-black rounded-full transition-transform duration-300 shadow-md"
                 :class="isAnnual ? 'translate-x-8' : 'translate-x-0'"></div>
          </button>
          <span class="text-sm font-bold" :class="isAnnual ? 'text-black' : 'text-gray-400'">Yearly</span>
        </div>
      </div>
      <div class="grid md:grid-cols-3 gap-8 max-w-5xl mx-auto">
        <!-- Free Plan -->
        <div class="p-8 border border-gray-100 rounded-3xl hover:shadow-xl transition duration-300 flex flex-col bg-gray-50">
          <h3 class="text-lg font-bold text-gray-500 mb-4">Free</h3>
          <div class="text-5xl font-black mb-2">$0</div>
          <p class="text-gray-500 text-sm mb-8">per user/month</p>
          <ul class="space-y-4 mb-8 flex-grow">
            <li class="flex items-center text-sm"><i class="fa-solid fa-check mr-3 text-[#ccf32f]"></i> Basic features</li>
            <li class="flex items-center text-sm"><i class="fa-solid fa-check mr-3 text-[#ccf32f]"></i> Up to 10 users</li>
          </ul>
          <button class="w-full py-3 rounded-xl border-2 border-black font-bold hover:bg-black hover:text-white transition">Get Started</button>
        </div>
        <!-- Pro Plan -->
        <div class="p-8 bg-[#ccf32f] rounded-3xl shadow-xl transform md:-translate-y-4 flex flex-col relative">
          <div class="absolute top-0 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-black text-white px-4 py-1 rounded-full text-xs font-bold uppercase">Popular</div>
          <h3 class="text-lg font-bold text-gray-800 mb-4">Pro</h3>
          <div class="text-5xl font-black mb-2">${{ isAnnual ? '79' : '99' }}</div>
          <p class="text-gray-800 text-sm mb-8">per user/month</p>
          <ul class="space-y-4 mb-8 flex-grow">
            <li class="flex items-center text-sm font-medium"><i class="fa-solid fa-check mr-3 text-white bg-black rounded-full p-1 text-[10px]"></i> Unlimited users</li>
            <li class="flex items-center text-sm font-medium"><i class="fa-solid fa-check mr-3 text-white bg-black rounded-full p-1 text-[10px]"></i> Advanced analytics</li>
            <li class="flex items-center text-sm font-medium"><i class="fa-solid fa-check mr-3 text-white bg-black rounded-full p-1 text-[10px]"></i> 24/7 Support</li>
          </ul>
          <button class="w-full py-3 rounded-xl bg-black text-white font-bold hover:bg-gray-800 transition shadow-lg">Get Started</button>
        </div>
        <!-- Enterprise Plan -->
        <div class="p-8 border border-gray-100 rounded-3xl hover:shadow-xl transition duration-300 flex flex-col bg-gray-50">
          <h3 class="text-lg font-bold text-[#ccf32f] mb-4">Enterprise</h3>
          <div class="text-5xl font-black mb-2">${{ isAnnual ? '899' : '999' }}</div>
          <p class="text-gray-500 text-sm mb-8">per user/month</p>
          <ul class="space-y-4 mb-8 flex-grow">
            <li class="flex items-center text-sm"><i class="fa-solid fa-check mr-3 text-[#ccf32f]"></i> Dedicated server</li>
            <li class="flex items-center text-sm"><i class="fa-solid fa-check mr-3 text-[#ccf32f]"></i> Custom integrations</li>
          </ul>
          <button class="w-full py-3 rounded-xl bg-[#ccf32f] text-black font-bold hover:bg-opacity-80 transition">Contact Us</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'

const isAnnual = ref(false)
</script>

