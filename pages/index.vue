<template>
  <div class="pt-20">
    <section class="screenSize flex items-center justify-center px-6">
      <div class="max-w-4xl mx-auto text-center">
        <h1 class="text-5xl md:text-7xl font-bold text-slate-900 mb-6 animate-slide-up">
          Salut ! Moi c'est <span class="text-slate-600">Simon CHEVRIER</span>
        </h1>
        <p class="text-xl md:text-2xl text-slate-600 mb-8 animate-slide-up-delay">
          Etudiant à EPITECH Strasbourg 
        </p>
        <div class="flex flex-wrap gap-4 justify-center animate-fade-in-delay">
          <NuxtLink 
            to="/contact"
            class="px-8 py-3 bg-slate-800 text-white rounded-lg hover:bg-slate-700 transition-all duration-300 hover:scale-105 hover:shadow-lg"
          >
            Me contacter
          </NuxtLink>
          <NuxtLink 
            to="/about"
            class="px-8 py-3 bg-white text-slate-800 border-2 border-slate-800 rounded-lg hover:bg-slate-800 hover:text-white transition-all duration-300 hover:scale-105"
          >
            En savoir plus
          </NuxtLink>
        </div>
      </div>

    <div class="absolute inset-0 z-0 pointer-events-none">
    <div class="shape w-16 h-16 bg-blue-300 rounded-full opacity-30 absolute"></div>
    <div class="shape w-20 h-20 bg-green-300 rounded-full opacity-30 absolute"></div>
    <div class="shape w-12 h-12 bg-yellow-300 rounded-full opacity-30 absolute"></div>

  </div>
    </section>

    <section class="py-20 px-6 bg-white">
      <div class="max-w-6xl mx-auto">
        <h2 class="text-4xl font-bold text-slate-900 mb-12 text-center">
          Compétences
        </h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div class="p-8 bg-slate-50 rounded-xl hover:shadow-lg transition-all duration-300 hover:translate-y-[-8px] group">
            <div class="w-12 h-12 bg-slate-50 rounded-lg mb-4 group-hover:scale-110 transition-transform duration-300">
              <img src="../assets/Tailwind CSS.png" alt="logo tailwind css" class="w-12 h-12 ">
            </div>
            <h3 class="text-xl font-semibold text-slate-900 mb-3">
              HTML/CSS 
            </h3>
            <p class="text-slate-600">
              Je conçois des sites web avec HTML, CSS et des frameworks modernes comme Nuxt.js et Vue 3.
            </p>
          </div>

          <div class="p-8 bg-slate-50 rounded-xl hover:shadow-lg transition-all duration-300 hover:translate-y-[-8px] group">
            <div class="w-12 h-12 bg-slate-50 rounded-lg mb-4 group-hover:scale-110 transition-transform duration-300">
              <img src="../assets/Java.png" alt="logo Java" class="w-12 h-12 ">
            </div>
            <h3 class="text-xl font-semibold text-slate-900 mb-3">
              Python, Java, Javascrypt et PHP
            </h3>
            <p class="text-slate-600">
              Je développe avec Python, Java, JavaScript et PHP pour créer des applications web dynamiques.
            </p>
          </div>

          <div class="p-8 bg-slate-50 rounded-xl hover:shadow-lg transition-all duration-300 hover:translate-y-[-8px] group">
            <div class="w-12 h-12 bg-slate-50 rounded-lg mb-4 group-hover:scale-110 transition-transform duration-300">
                <img src="../assets/collaboration.png" alt="logo Java" class="w-12 h-12 ">
            </div>
            <h3 class="text-xl font-semibold text-slate-900 mb-3">
              Mes softskills
            </h3>
            <p class="text-slate-600">
              J’allie rigueur, sens du relationnel et esprit d’équipe.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="py-20 px-6 bg-slate-50">
<div class="max-w-6xl mx-auto">
  <h2 class="text-4xl font-bold text-slate-900 mb-12 text-center">
    Projets récents
  </h2>
  <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
    <div class="bg-white rounded-xl overflow-hidden hover:shadow-xl transition-all duration-300 hover:scale-105 group">
      <a href="https://github.com/Simon-chevrier/Go-Job">
      <div class="h-48 bg-slate-200 group-hover:bg-slate-300 transition-colors duration-300 flex items-center justify-center">
        <img src="../assets/GoJob.png" alt="page home go job" class="w-full h-full object-cover">
      </div>
      <div class="p-6">
        <h3 class="text-2xl font-semibold text-slate-900 mb-2">
          Go-job
        </h3>
        <p class="text-slate-600 mb-4">
          Go-job est un jobboard fais en équipe de deux dans lequel il est possible de faire toutes les fonctionnalités nécéssaires à la recherche d'emploi
        </p>
        <div class="flex gap-2 flex-wrap">
          <span class="px-3 py-1 bg-slate-100 text-slate-700 text-sm rounded-full">Flask.python</span>
          <span class="px-3 py-1 bg-slate-100 text-slate-700 text-sm rounded-full">Vue 3</span>
        </div>
      </div>
      </a>
    </div>
    <div class="bg-white rounded-xl overflow-hidden hover:shadow-xl transition-all duration-300 hover:scale-105 group">
      <div class="h-48 bg-slate-200 group-hover:bg-slate-300 transition-colors duration-300">
        <img src="../assets/Epimon.png" alt="image décorative" class="w-full h-full object-cover">
      </div>
      <div class="p-6">
        <h3 class="text-2xl font-semibold text-slate-900 mb-2">
          Epimon
        </h3>
        <p class="text-slate-600 mb-4">
          Epimon est un jeu codé en java, inspiré de pokémon conçu par moi et deux de mes amis dans lequel il est possible de choisir son starter et combattre des dresseurs.
        </p>
        <div class="flex gap-2 flex-wrap">
          <span class="px-3 py-1 bg-slate-100 text-slate-700 text-sm rounded-full">Vue 3</span>
        </div>
      </div>
    </div>
  </div>
</div>
    </section>
  </div>
</template>

<script setup>
import { onMounted } from 'vue'
import * as animejs from 'animejs'
const anime = animejs.default || animejs

onMounted(() => {
  anime({
    targets: '.shape',
    translateX: () => Math.random() * 200 - 100,
    translateY: () => Math.random() * 200 - 100,
    rotate: () => Math.random() * 360 - 180,
    duration: () => Math.random() * 4000 + 4000,
    direction: 'alternate',
    loop: true,
    easing: 'easeInOutSine'
  })
})
</script>

<style scoped>
@keyframes slide-up {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.shape {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.animate-slide-up {
  animation: slide-up 0.8s ease-out;
}

.animate-slide-up-delay {
  animation: slide-up 0.8s ease-out 0.2s both;
}

.animate-fade-in-delay {
  animation: slide-up 0.8s ease-out 0.4s both;
}
.screenSize {
  height: calc(var(--framer-viewport-height, 100vh)*1);
}
</style>