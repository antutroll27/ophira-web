<template>
  <section id="faq" class="py-24 bg-gray-50">
    <div class="container mx-auto px-6 grid md:grid-cols-12 gap-12">
      <div class="md:col-span-4">
        <h2 class="text-4xl font-black mb-4">FAQs</h2>
        <p class="text-gray-600 mb-6">
          Everything you need to know about the product and billing. Can't find the answer you're looking for? Please chat to our friendly team.
        </p>
      </div>
      <div class="md:col-span-8">
        <div class="space-y-4">
          <div v-for="(item, index) in faqs" :key="index" class="bg-white rounded-xl shadow-sm overflow-hidden">
            <button @click="toggleFaq(index)" class="w-full px-6 py-4 text-left flex justify-between items-center focus:outline-none">
              <span class="font-bold">{{ item.question }}</span>
              <i class="fa-solid transition-transform duration-300" :class="item.isOpen ? 'fa-minus text-[#ccf32f]' : 'fa-plus text-gray-400'"></i>
            </button>
            <div v-show="item.isOpen" class="px-6 pb-4 text-gray-600">
              {{ item.answer }}
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'

const faqs = ref([
  { question: "Is there a free trial available?", answer: "Yes, you can try us for free for 30 days. If you want, we'll provide you with a free, personalized 30-minute onboarding call to get you up and running as soon as possible.", isOpen: true },
  { question: "Can I change my plan later?", answer: "Absolutely. You can upgrade or downgrade your plan at any time from your account settings.", isOpen: false },
  { question: "What is your cancellation policy?", answer: "You can cancel at any time. There are no cancellation fees, though we do not offer refunds for partial months.", isOpen: false },
  { question: "Do you offer enterprise pricing?", answer: "Yes, for teams larger than 50 people, please contact our sales team for a custom quote.", isOpen: false },
  { question: "How does billing work?", answer: "We bill monthly or annually depending on your preference. Annual plans come with a significant discount.", isOpen: false }
])

const toggleFaq = (index) => {
  faqs.value[index].isOpen = !faqs.value[index].isOpen
}
</script>

