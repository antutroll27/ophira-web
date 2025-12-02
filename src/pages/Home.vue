<template>
  <div>
    <!-- Navigation -->
    <Navbar :is-scrolled="isScrolled" @toggle-mobile-menu="mobileMenuOpen = !mobileMenuOpen" />
    
    <!-- Mobile Menu Overlay -->
    <MobileMenu :is-open="mobileMenuOpen" @close="mobileMenuOpen = false" />
    
    <!-- Hero Section -->
    <Hero />
    
    <!-- Product Description Section -->
    <ProductSection />
    
    <!-- Video Section -->
    <VideoSection />
    
    <!-- About / How We Started -->
    <AboutSection />
    
    <!-- Features -->
    <FeaturesSection />
    
    <!-- Pricing -->
    <PricingSection />
    
    <!-- Testimonial -->
    <TestimonialSection />
    
    <!-- FAQ -->
    <FAQSection />
    
    <!-- Footer -->
    <FooterSection />
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'
import Navbar from '../components/Navbar.vue'
import MobileMenu from '../components/MobileMenu.vue'
import Hero from '../components/Hero.vue'
import ProductSection from '../components/ProductSection.vue'
import VideoSection from '../components/VideoSection.vue'
import AboutSection from '../components/AboutSection.vue'
import FeaturesSection from '../components/FeaturesSection.vue'
import PricingSection from '../components/PricingSection.vue'
import TestimonialSection from '../components/TestimonialSection.vue'
import FAQSection from '../components/FAQSection.vue'
import FooterSection from '../components/FooterSection.vue'

const isScrolled = ref(false)
const mobileMenuOpen = ref(false)

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

