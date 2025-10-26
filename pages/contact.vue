<template>
  <div class="pt-20 min-h-screen">
    <section class="py-20 px-6 bg-white">
      <div class="max-w-4xl mx-auto">
        <h1 class="text-5xl font-bold text-slate-900 mb-6 animate-fade-in">
          Contactez-moi
        </h1>
        <p class="text-xl text-slate-600 mb-12 animate-fade-in-delay">
          Une question ? Un projet ? N'hésitez pas à me contacter !
        </p>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
          <div class="animate-slide-left">
            <form @submit.prevent="handleSubmit" class="space-y-6">
              <div>
                <label class="block text-slate-700 font-medium mb-2">
                  Nom
                </label>
                <input
                  v-model="form.name"
                  type="text"
                  required
                  class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-lg focus:outline-none focus:ring-2 focus:ring-slate-400 transition-all duration-300"
                  placeholder="Votre nom"
                />
              </div>

              <div>
                <label class="block text-slate-700 font-medium mb-2">
                  Email
                </label>
                <input
                  v-model="form.email"
                  type="email"
                  required
                  class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-lg focus:outline-none focus:ring-2 focus:ring-slate-400 transition-all duration-300"
                  placeholder="votre@email.com"
                />
              </div>

              <div>
                <label class="block text-slate-700 font-medium mb-2">
                  Sujet
                </label>
                <input
                  v-model="form.subject"
                  type="text"
                  required
                  class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-lg focus:outline-none focus:ring-2 focus:ring-slate-400 transition-all duration-300"
                  placeholder="Objet"
                />
              </div>

              <div>
                <label class="block text-slate-700 font-medium mb-2">
                  Message
                </label>
                <textarea
                  v-model="form.message"
                  required
                  rows="6"
                  class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-lg focus:outline-none focus:ring-2 focus:ring-slate-400 transition-all duration-300 resize-none"
                  placeholder="Votre message..."
                ></textarea>
              </div>

              <button
                type="submit"
                class="w-full px-8 py-4 bg-slate-800 text-white rounded-lg hover:bg-slate-700 transition-all duration-300 hover:scale-105 hover:shadow-lg font-medium"
              >
                Envoyer
              </button>
            </form>

            <div
              v-if="showSuccess"
              class="mt-6 p-4 bg-green-50 border border-green-200 rounded-lg text-green-800 animate-fade-in"
            >
              Message envoyé avec succès ! 
            </div>
          </div>

          <div class="space-y-8 animate-slide-right">
            <div>
              <h2 class="text-2xl font-semibold text-slate-900 mb-6">
                Autres moyens de me contacter
              </h2>
              
              <div class="space-y-6">
                <div class="flex items-start gap-4 p-4 bg-slate-50 rounded-lg hover:bg-slate-100 transition-colors duration-300">
                  <div class="w-12 h-12 bg-slate-800 rounded-lg flex items-center justify-center flex-shrink-0">
                    <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                    </svg>
                  </div>
                  <div>
                    <h3 class="font-semibold text-slate-900 mb-1">Email</h3>
                    <a href="mailto:simon.chevrier@epitech.eu" class="text-slate-600 hover:text-slate-900 transition-colors">
                      simon.chevrier@epitech.eu
                    </a>
                  </div>
                </div>

                <div class="flex items-start gap-4 p-4 bg-slate-50 rounded-lg hover:bg-slate-100 transition-colors duration-300">
                  <div class="w-12 h-12 bg-slate-700 rounded-lg flex items-center justify-center flex-shrink-0">
                    <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 24 24">
                      <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
                    </svg>
                  </div>
                  <div>
                    <h3 class="font-semibold text-slate-900 mb-1">LinkedIn</h3>
                    <a href="https://www.linkedin.com/in/simon-chevrier" target="_blank" class="text-slate-600 hover:text-slate-900 transition-colors">
                      Simon CHEVRIER
                    </a>
                  </div>
                </div>

                <div class="flex items-start gap-4 p-4 bg-slate-50 rounded-lg hover:bg-slate-100 transition-colors duration-300">
                  <div class="w-12 h-12 bg-slate-600 rounded-lg flex items-center justify-center flex-shrink-0">
                    <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 24 24">
                      <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
                    </svg>
                  </div>
                  <div>
                    <h3 class="font-semibold text-slate-900 mb-1">GitHub</h3>
                    <a href="https://github.com/Simon-chevrier" target="_blank" class="text-slate-600 hover:text-slate-900 transition-colors">
                      Simon-chevrier
                    </a>
                  </div>
                </div>
              </div>
            </div>

            <div class="p-6 bg-slate-800 text-white rounded-xl">
              <h3 class="text-xl font-semibold mb-3">Disponibilité</h3>
              <p class="text-slate-300">
                Je suis actuellement disponible pour de nouveaux projets et activement en recherche d'alternance pour Janvier 2026.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import { ref, reactive } from 'vue'
import emailjs from '@emailjs/browser'

const form = reactive({
  name: '',
  email: '',
  subject: '',
  message: ''
})

const showSuccess = ref(false)

const handleSubmit = async () => {
  try {
    await emailjs.send(
      import.meta.env.NUXT_PUBLIC_EMAILJS_SERVICE_ID || 'service_ftr6m52',
      import.meta.env.NUXT_PUBLIC_EMAILJS_TEMPLATE_ID || 'template_ursiptb',
      {
        name: form.name,
        email: form.email,
        subject: form.subject,
        message: form.message
      },
      import.meta.env.NUXT_PUBLIC_EMAILJS_PUBLIC_KEY || 'lO6guEu1XbocuPwi0'
    )
  
    
    showSuccess.value = true
    
    form.name = ''
    form.email = ''
    form.subject = ''
    form.message = ''
    
    setTimeout(() => {
      showSuccess.value = false
    }, 5000)
    
  } catch (error) {
    console.error('Erreur:', error)
    alert('Erreur lors de l\'envoi. Réessayez.')
  }
}
</script>

<style scoped>
@keyframes fade-in {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@keyframes fade-in-delay {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@keyframes slide-left {
  from {
    opacity: 0;
    transform: translateX(-30px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes slide-right {
  from {
    opacity: 0;
    transform: translateX(30px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

.animate-fade-in {
  animation: fade-in 0.8s ease-out;
}

.animate-fade-in-delay {
  animation: fade-in-delay 0.8s ease-out 0.2s both;
}

.animate-slide-left {
  animation: slide-left 0.8s ease-out 0.3s both;
}

.animate-slide-right {
  animation: slide-right 0.8s ease-out 0.4s both;
}
</style>