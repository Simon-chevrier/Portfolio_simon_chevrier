<template>
  <nav class="fixed top-0 left-0 right-0 z-50 bg-white/80 backdrop-blur-md shadow-sm">
    <div class="max-w-6xl mx-auto px-6 py-4">
      <div class="flex items-center justify-between">
        <NuxtLink 
          to="/" 
          class="text-xl font-bold text-slate-800 hover:text-slate-600 transition-colors duration-300"
        >
          Simon CHEVRIER
        </NuxtLink>

        <div class="hidden md:flex items-center gap-8">
          <NuxtLink 
            to="/" 
            class="text-slate-700 hover:text-slate-900 transition-all duration-300 hover:translate-y-[-2px]"
            active-class="text-slate-900 font-semibold"
          >
            Accueil
          </NuxtLink>
          <NuxtLink 
            to="/about" 
            class="text-slate-700 hover:text-slate-900 transition-all duration-300 hover:translate-y-[-2px]"
            active-class="text-slate-900 font-semibold"
          >
            À propos
          </NuxtLink>
          <NuxtLink 
            to="/contact" 
            class="text-slate-700 hover:text-slate-900 transition-all duration-300 hover:translate-y-[-2px]"
            active-class="text-slate-900 font-semibold"
          >
            Contact
          </NuxtLink>
        </div>

        <button 
          @click="toggleMenu"
          class="md:hidden text-slate-700 hover:text-slate-900 transition-colors"
        >
          <svg 
            v-if="!isMenuOpen" 
            class="w-6 h-6" 
            fill="none" 
            stroke="currentColor" 
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
          <svg 
            v-else 
            class="w-6 h-6" 
            fill="none" 
            stroke="currentColor" 
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
      </div>

      <div 
        v-if="isMenuOpen"
        class="md:hidden mt-4 pb-4 flex flex-col gap-4 animate-fade-in"
      >
        <NuxtLink 
          to="/" 
          @click="closeMenu"
          class="text-slate-700 hover:text-slate-900 transition-colors py-2"
          active-class="text-slate-900 font-semibold"
        >
          Accueil
        </NuxtLink>
        <NuxtLink 
          to="/about" 
          @click="closeMenu"
          class="text-slate-700 hover:text-slate-900 transition-colors py-2"
          active-class="text-slate-900 font-semibold"
        >
          À propos
        </NuxtLink>
        <NuxtLink 
          to="/contact" 
          @click="closeMenu"
          class="text-slate-700 hover:text-slate-900 transition-colors py-2"
          active-class="text-slate-900 font-semibold"
        >
          Contact
        </NuxtLink>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}

const closeMenu = () => {
  isMenuOpen.value = false
}
</script>

<style scoped>
@keyframes fade-in {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.animate-fade-in {
  animation: fade-in 0.3s ease-out;
}
</style>