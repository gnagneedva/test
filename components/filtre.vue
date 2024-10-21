<template>
    <button class="lg:hidden gap-6 fixed top-7 z-50 bg-slate-400 p-2 rounded-md text-first right-7 flex-col flex" v-on:click="toggleClass">Filtrer</button>
  <div
  :class="[ classActive ? ' translate-1/4' : ' -translate-x-[800%]  ']"
  class="bg-neutral-100 fixed w-5/6 left-1  top-0 lg:hidden transition ease-in-out flex-col flex gap-6 rounded p-4">
    <div class="w-full border-b-2 pt-5 pb-4 h-fit border-black">
      <span class="font-bold text-2xl">FILTRE</span>
    </div>
    <div class="w-full flex justify-start gap-2 items-center">
      <span class="p-2 h-fit bg-white rounded-xl text-sm"
        >Produits agricoles</span
      >
      <span class="p-2 bg-white rounded-xl text-sm">Intrants</span>
    </div>
    <div class="flex flex-col w-full">
      <label for="">Rechercher</label>
      <input class="outline-none p-2" type="text" />
    </div>
    <div class="flex flex-col w-full">
      <span for="">Les offres</span>
      <div class="w-full flex flex-col justify-center gap-2 items-start">
        <span class="p-2 h-fit bg-white rounded-xl text-sm">Ofre de vente</span>
        <span class="p-2 bg-white rounded-xl text-sm"
          >Offre achat & préachat</span
        >
      </div>
    </div>
    <div class="flex flex-col w-full">
      <div class="w-full flex justify-between">
        <span for="">Les offres</span>
        <span for="" class="text-green-800 pb-2">Reinitialiser</span>
      </div>
      <div class="w-full flex justify-start flex-wrap gap-3">
        <span class="p-2 h-fit bg-green-800 text-white rounded-xl text-sm"
          >Tous</span
        >
        <span class="p-2 bg-white rounded-xl text-sm">Oléagineux</span>
        <span class="p-2 h-fit bg-white rounded-xl text-sm">Animaux</span>
        <span class="p-2 bg-white rounded-xl text-sm">Hlieutiques</span>
        <span class="p-2 h-fit bg-white rounded-xl text-sm">Légumineux</span>
        <span class="p-2 bg-white rounded-xl text-sm">Céréales</span>
        <span class="p-2 bg-white rounded-xl text-sm">Tubercules</span>
      </div>
    </div>
    <div class="flex flex-col w-full">
      <div class="w-full flex justify-between">
        <span for="">Evaluations clients</span>
        <span for="" class="text-green-800 pb-2">Reinitialiser</span>
      </div>
      <div class="w-full flex justify-start flex-wrap gap-2">
        <span class="p-2 text-yellow-500 h-fit bg-green-800 rounded-xl text-sm"
          >&#9733;</span
        >
        <span class="p-2 bg-white text-yellow-500 rounded-xl text-sm"
          >&#9733; &#9733;</span
        >
        <span class="p-2 h-fit bg-white text-yellow-500 rounded-xl text-sm"
          >&#9733; &#9733; &#9733;</span
        >
        <span class="p-2 bg-white text-yellow-500 rounded-xl text-sm"
          >&#9733; &#9733; &#9733; &#9733;</span
        >
        <span class="p-2 h-fit bg-white text-yellow-500 rounded-xl text-sm"
          >&#9733; &#9733; &#9733; &#9733; &#9733;</span
        >
      </div>
    </div>
    <div class="flex flex-col w-full">
      <div class="w-full flex justify-between">
        <span for="">Localisation</span>
        <span for="" class="text-green-800 pb-2">Reinitialiser</span>
      </div>
      <div class="w-full grid grid-cols-2 justify-start flex-wrap gap-2">
        <div
          class="p-2 h-fit flex justify-between col-span-2 bg-white text-black text-sm"
        >
          <span>Choisir la région</span>
          <select class="outline-none" name="" id="">
            <option value="ville"></option>
            <option value="ville">ville</option>
            <option value="ville">ville</option>
            <option value="ville">ville</option>
          </select>
        </div>
        <div
          class="p-2 grid grid-cols-2 h-fit justify-between col-span-1 bg-white text-black text-sm">
          <span>Du</span>
          <input type="date" class="w-full h-full" name="" id="">
        </div>
        <div
          class="p-2 grid grid-cols-2 h-fit justify-between col-span-1 bg-white text-black text-sm">
          <span>Au</span>
          <input type="date" class="w-full h-full" name="" id="">
        </div>
        
      </div>
    </div>
    <div class="flex flex-col w-full">
      
      <div class="w-full grid grid-cols-2 justify-start flex-wrap gap-2">
        <button class="p-2  col-span-1 bg-green-800 text-white text-sm">
          Filtrer
        </button>
        <button class="p-2  col-span-1 bg-red-800 text-white text-sm">
          Reinitialiser
        </button>
        <button class="p-2 h-fit bg-green-800 text-white col-span-2   text-sm">
          Consulter le prix du marché
        </button>
      </div>
    </div>
  </div>


  <div
  
  class="bg-neutral-100  hidden flex-col lg:flex gap-6   rounded p-4">
    <div class="w-full border-b-2 pt-5 pb-4 h-fit border-black">
      <span class="font-bold text-2xl">FILTRE</span>
    </div>
    <div class="w-full flex justify-start gap-2 items-center">
      <span class="p-2 h-fit bg-white rounded-xl text-sm"
        >Produits agricoles</span
      >
      <span class="p-2 bg-white rounded-xl text-sm">Intrants</span>
    </div>
    <div class="flex flex-col w-full">
      <label for="">Rechercher</label>
      <input class="outline-none p-2" type="text" />
    </div>
    <div class="flex flex-col w-full">
      <span for="">Les offres</span>
      <div class="w-full flex flex-col justify-center gap-2 items-start">
        <span class="p-2 h-fit bg-white rounded-xl text-sm">Ofre de vente</span>
        <span class="p-2 bg-white rounded-xl text-sm"
          >Offre achat & préachat</span
        >
      </div>
    </div>
    <div class="flex flex-col w-full">
      <div class="w-full flex justify-between">
        <span for="">Les offres</span>
        <span for="" class="text-green-800 pb-2">Reinitialiser</span>
      </div>
      <div class="w-full flex justify-start flex-wrap gap-3">
        <span class="p-2 h-fit bg-green-800 text-white rounded-xl text-sm"
          >Tous</span
        >
        <span class="p-2 bg-white rounded-xl text-sm">Oléagineux</span>
        <span class="p-2 h-fit bg-white rounded-xl text-sm">Animaux</span>
        <span class="p-2 bg-white rounded-xl text-sm">Hlieutiques</span>
        <span class="p-2 h-fit bg-white rounded-xl text-sm">Légumineux</span>
        <span class="p-2 bg-white rounded-xl text-sm">Céréales</span>
        <span class="p-2 bg-white rounded-xl text-sm">Tubercules</span>
      </div>
    </div>
    <div class="flex flex-col w-full">
      <div class="w-full flex justify-between">
        <span for="">Evaluations clients</span>
        <span for="" class="text-green-800 pb-2">Reinitialiser</span>
      </div>
      <div class="w-full flex justify-start flex-wrap gap-2">
        <span class="p-2 text-yellow-500 h-fit bg-green-800 rounded-xl text-sm"
          >&#9733;</span
        >
        <span class="p-2 bg-white text-yellow-500 rounded-xl text-sm"
          >&#9733; &#9733;</span
        >
        <span class="p-2 h-fit bg-white text-yellow-500 rounded-xl text-sm"
          >&#9733; &#9733; &#9733;</span
        >
        <span class="p-2 bg-white text-yellow-500 rounded-xl text-sm"
          >&#9733; &#9733; &#9733; &#9733;</span
        >
        <span class="p-2 h-fit bg-white text-yellow-500 rounded-xl text-sm"
          >&#9733; &#9733; &#9733; &#9733; &#9733;</span
        >
      </div>
    </div>
    <div class="flex flex-col w-full">
      <div class="w-full flex justify-between">
        <span for="">Localisation</span>
        <span for="" class="text-green-800 pb-2">Reinitialiser</span>
      </div>
      <div class="w-full grid grid-cols-2 justify-start flex-wrap gap-2">
        <div
          class="p-2 h-fit flex justify-between col-span-2 bg-white text-black text-sm"
        >
          <span>Choisir la région</span>
          <select class="outline-none" name="" id="">
            <option value="ville"></option>
            <option value="ville">ville</option>
            <option value="ville">ville</option>
            <option value="ville">ville</option>
          </select>
        </div>
        <div
          class="p-2 grid grid-cols-2 h-fit justify-between col-span-1 bg-white text-black text-sm">
          <span>Du</span>
          <input type="date" class="w-full h-full" name="" id="">
        </div>
        <div
          class="p-2 grid grid-cols-2 h-fit justify-between col-span-1 bg-white text-black text-sm">
          <span>Au</span>
          <input type="date" class="w-full h-full" name="" id="">
        </div>
        
      </div>
    </div>
    <div class="flex flex-col w-full">
      
      <div class="w-full grid grid-cols-2 justify-start flex-wrap gap-2">
        <button class="p-2  col-span-1 bg-green-800 text-white text-sm">
          Filtrer
        </button>
        <button class="p-2  col-span-1 bg-red-800 text-white text-sm">
          Reinitialiser
        </button>
        <button class="p-2 h-fit bg-green-800 text-white col-span-2   text-sm">
          Consulter le prix du marché
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
    const classActive = ref(false)

// Fonction pour ajouter ou retirer la classe Tailwind
const toggleClass = () => {
  classActive.value = !classActive.value
}
</script>

<style scoped>
span {
  font-size: 12px !important;
}
</style>
