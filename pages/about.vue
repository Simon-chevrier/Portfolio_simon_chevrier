<template>
  <div class="pt-20 min-h-screen">
    <section class="py-20 px-6 bg-white">
      <div class="max-w-4xl mx-auto">
        <h1 class="text-5xl font-bold text-slate-900 mb-8 animate-fade-in">
          À propos de moi
        </h1>
        <div class="flex flex-col md:flex-row gap-12 items-start">
          <div class="w-full md:w-1/3">
            <div class="aspect-square rounded-2xl hover:scale-105 transition-transform duration-300">
                <img src="../assets/avatar.png" alt="avatar de ma personne">
            </div>
          </div>
          
          <div class="w-full  md:w-2/3 space-y-6 text-slate-700 leading-relaxed animate-slide-in">
            <p class="text-xl">
              Salut ! moi c'est <strong class="text-slate-900">Simon</strong>, 
              un étudiant en pré-Master of Science à Epitech Strasbourg passionné par le sport, les jeux vidéos et la MUSIQUE !
            </p>
            <p class="text-xl">
              Avec 3 années d'expérience dans la chimie, j'ai développé 
              des compétences solides tels que le travail d'équipe, la rigueur et la résolution de problème complexe.
              Je me suis ensuite réorienté vers le domaine passionnant qu'est l'informatique. Mon approche 
              combine créativité et technique pour créer des solutions innovantes.
            </p>
            <p class="mt-3 text-xl">
            Actuellement, je suis une formation passionnante à Epitech, où j’apprends à concevoir et développer des projets concrets 
            en informatique. Ce cursus me permet de renforcer mes compétences en programmation, en gestion d’équipe et en 
            résolution de problèmes tout en cultivant une vraie autonomie technique.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="py-20 px-6 bg-slate-50">
      <div class="max-w-4xl mx-auto">
        <h2 class="text-4xl font-bold text-slate-900 mb-12">
          Mon parcours
        </h2>
        <div class="space-y-8">
          <div class="flex gap-6 group">
            <div class="flex flex-col items-center">
              <div class="w-4 h-4 bg-slate-800 rounded-full group-hover:scale-150 transition-transform duration-300"></div>
              <div class="w-0.5 h-full bg-slate-300 mt-2"></div>
            </div>
            <div class="pb-12 flex-1">
              <span class="text-slate-500 text-sm">2025-2028</span>
              <h3 class="text-2xl font-semibold text-slate-900 mt-2 mb-3">
                Master of Science
              </h3>
              <p class="text-slate-600 mb-2">
                <strong>Epitech Strasbourg</strong>
              </p>
              <p class="text-slate-600">
                Je suis actuellement en pré-Master à Epitech, une formation en trois ans qui me permet 
                de me former et d'approfondir mes compétences en développement, en gestion de projet
                 et en innovation technologique à travers des projets concrets 
                 et un apprentissage centré sur la pratique.
              </p>
            </div>
          </div>

          <div class="flex gap-6 group">
            <div class="flex flex-col items-center">
              <div class="w-4 h-4 bg-slate-700 rounded-full group-hover:scale-150 transition-transform duration-300"></div>
              <div class="w-0.5 h-full bg-slate-300 mt-2"></div>
            </div>
            <div class="pb-12 flex-1">
              <span class="text-slate-500 text-sm">2022-2025</span>
              <h3 class="text-2xl font-semibold text-slate-900 mt-2 mb-3">
                Diplôme de BUT chimie spécialité chimie industrielle
              </h3>
              <p class="text-slate-600 mb-2">
                <strong>IUT Robert-Schuman, Illkirch-Graffenstaden, 67411</strong>
              </p>
              <p class="text-slate-600">
                Diplomé d'un BUT Chimie, spécialité Chimie industrielle, où j’ai appris
                 à allier rigueur scientifique, maîtrise des procédés chimiques et contrôle des paramètres industriels,
                  tout en développant un vrai sens du travail en équipe dans des environnements techniques exigeants.
              </p>
            </div>
          </div>

          <div class="flex gap-6 group">
            <div class="flex flex-col items-center">
              <div class="w-4 h-4 bg-slate-600 rounded-full group-hover:scale-150 transition-transform duration-300"></div>
            </div>
            <div class="flex-1">
              <span class="text-slate-500 text-sm">2022</span>
              <h3 class="text-2xl font-semibold text-slate-900 mt-2 mb-3">
                Baccalauréat spécialités physique-chimie et Mathématiques
              </h3>
              <p class="text-slate-600 mb-2">
                <strong>Lycée Beau Jardin, Saint-Dié-des-Vosges 88100 </strong>
              </p>
              <p class="text-slate-600">
                Diplôme obtenu mention assez bien.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="py-20 px-6 bg-white">
      <div class="max-w-4xl mx-auto">
        <h2 class="text-4xl font-bold text-slate-900 mb-12">
          Compétences techniques
        </h2>
        <div class="grid grid-cols-2 md:grid-cols-4 gap-6">
          <div class="p-6 bg-slate-50 rounded-xl text-center hover:bg-slate-100 transition-all duration-300 hover:scale-105">
            <p class="text-slate-800 font-medium">HTML</p>
          </div>
          <div class="p-6 bg-slate-50 rounded-xl text-center hover:bg-slate-100 transition-all duration-300 hover:scale-105">
            <p class="text-slate-800 font-medium">CSS</p>
          </div>
          <div class="p-6 bg-slate-50 rounded-xl text-center hover:bg-slate-100 transition-all duration-300 hover:scale-105">
            <p class="text-slate-800 font-medium">Python</p>
          </div>
          <div class="p-6 bg-slate-50 rounded-xl text-center hover:bg-slate-100 transition-all duration-300 hover:scale-105">
            <p class="text-slate-800 font-medium">Communication</p>
          </div>
          <div class="p-6 bg-slate-50 rounded-xl text-center hover:bg-slate-100 transition-all duration-300 hover:scale-105">
            <p class="text-slate-800 font-medium">PHP</p>
          </div>
          <div class="p-6 bg-slate-50 rounded-xl text-center hover:bg-slate-100 transition-all duration-300 hover:scale-105">
            <p class="text-slate-800 font-medium">Java</p>
          </div>
          <div class="p-6 bg-slate-50 rounded-xl text-center hover:bg-slate-100 transition-all duration-300 hover:scale-105">
            <p class="text-slate-800 font-medium">Javascript</p>
          </div>
          <div class="p-6 bg-slate-50 rounded-xl text-center hover:bg-slate-100 transition-all duration-300 hover:scale-105">
            <p class="text-slate-800 font-medium">Rigueur</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
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

@keyframes slide-in {
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

.animate-slide-in {
  animation: slide-in 0.8s ease-out 0.3s both;
}
</style>