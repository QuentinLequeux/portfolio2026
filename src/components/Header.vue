<script lang="ts">
import {defineComponent} from 'vue'

export default defineComponent({
  name: "Header"
})
</script>

<template>
  <header class="fixed top-10 left-1/2 -translate-x-1/2 bg-white w-[90%] h-15 shadow-lg rounded-xl flex items-center p-6">
    <h1 class="sr-only" aria-level="1" role="heading">
      Quentin Lequeux
    </h1>
    <nav class="flex w-full justify-between">
      <h2 class="sr-only" aria-level="2" role="heading">
        Navigation principale
      </h2>
      <a href="/" title="Vers la page d'accueil" class="font-bold">
        Quentin Lequeux
      </a>
      <div class="flex max-sm:hidden">
        <a href="/about" title="Vers la page À propos" class="font-semibold mr-4 hover:text-red-500">
          À&nbsp;propos
        </a>
        <a href="/projects" title="Vers la page Projets" class="font-semibold mr-4 hover:text-red-500">
          Projets
        </a>
        <div class="relative">
          <a href="/contact" title="Vers la page Contact" class="font-semibold hover:text-red-500">
            Contact
          </a>
          <span class="absolute -top-0.5 -right-3 flex h-2.5 w-2.5">
            <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-green-400"/>
            <span class="relative inline-flex rounded-full h-2.5 w-2.5 bg-green-500"/>
          </span>
        </div>
      </div>
    </nav>
  </header>
</template>

<!-- TODO : Burger-menu -->
