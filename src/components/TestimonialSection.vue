<template>
  <section class="py-24 bg-white text-center">
    <div class="container mx-auto px-6">
      <h2 class="text-3xl font-black mb-12">Trusted by Businesses & <br> Lorem Ipsum</h2>
      
      <div class="max-w-3xl mx-auto">
        <div class="mb-8">
          <i class="fa-solid fa-quote-left text-4xl text-[#ccf32f] mb-6"></i>
          <p class="text-2xl font-medium leading-relaxed">
            "{{ testimonials[activeTestimonial].text }}"
          </p>
        </div>
        
        <div class="flex items-center justify-center space-x-4 mb-8">
          <div class="w-12 h-12 bg-gray-200 rounded-full overflow-hidden">
            <img :src="testimonials[activeTestimonial].image" class="w-full h-full object-cover">
          </div>
          <div class="text-left">
            <div class="font-bold">{{ testimonials[activeTestimonial].name }}</div>
            <div class="text-xs text-gray-500">{{ testimonials[activeTestimonial].role }}</div>
          </div>
        </div>
        <!-- Dots -->
        <div class="flex justify-center space-x-2">
          <button v-for="(t, index) in testimonials" :key="index" 
                  @click="activeTestimonial = index"
                  class="w-3 h-3 rounded-full transition-all"
                  :class="activeTestimonial === index ? 'bg-[#ccf32f] w-6' : 'bg-gray-200'">
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'

const activeTestimonial = ref(0)

const testimonials = [
  { 
    name: "Alex Rivera", 
    role: "CEO at TechFlow", 
    text: "Ophira completely transformed how we handle our internal workflows. The UI is stunning and the performance is unmatched.",
    image: "https://randomuser.me/api/portraits/men/32.jpg"
  },
  { 
    name: "Sarah Chen", 
    role: "Product Manager", 
    text: "I've used many tools before, but nothing comes close to the simplicity and power of Ophira. Highly recommended!",
    image: "https://randomuser.me/api/portraits/women/44.jpg"
  },
  { 
    name: "Michael Ross", 
    role: "Freelancer", 
    text: "The pricing is unbeatable for the value you get. The customer support team is also incredibly responsive.",
    image: "https://randomuser.me/api/portraits/men/85.jpg"
  }
]
</script>

