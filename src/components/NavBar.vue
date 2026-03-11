<template>
  <nav class="fixed top-0 left-0 right-0 z-50 transition-all duration-500 py-7 px-[4vw]">

    <div class="max-w-[120rem] mx-auto flex justify-between items-center">

      <a
        href="#"
        class="font-extrabold text-sm uppercase tracking-[2px] text-primary transition-colors duration-500"
      >
        Estrategista.Digital
      </a>

      <div class="hidden md:flex items-center gap-8">

        <a href="#servicos"
          class="text-xs font-semibold uppercase tracking-[1.5px] text-primary transition-colors duration-300 hover:text-[#e2aef0]">
          Serviços
        </a>

        <a href="#portfolio"
          class="text-xs font-semibold uppercase tracking-[1.5px] text-primary transition-colors duration-300 hover:text-[#e2aef0]">
          Portfólio
        </a>

        <a href="#processo"
          class="text-xs font-semibold uppercase tracking-[1.5px] text-primary transition-colors duration-300 hover:text-[#e2aef0]">
          Processo
        </a>

        <a href="#contato"
          class="text-xs font-semibold uppercase tracking-[1.5px] text-primary transition-colors duration-300 hover:text-[#e2aef0]">
          Contato
        </a>

        <a
          href="#contato"
          class="px-6 py-3 text-xs font-semibold uppercase tracking-[1.5px] text-white bg-primary transition-all duration-300 hover:-translate-y-0.5 min-h-[48px]"
        >
          Falar Comigo
        </a>

      </div>

      <button
        class="md:hidden p-2 text-primary"
        aria-label="Menu"
      >
        ☰
      </button>

    </div>

  </nav>
</template>

<script setup>
import { ref } from "vue"

const menuOpen = ref(false)

function toggleMenu(){
  menuOpen.value = !menuOpen.value
}
</script>

<!-- <style scoped>

.nav-link{
  @apply text-xs font-semibold uppercase tracking-[1.5px] text-primary transition-colors duration-300 hover:text-[#e2aef0];
}

.cta-button{
  @apply px-6 py-3 text-xs font-semibold uppercase tracking-[1.5px] text-white bg-primary transition-all duration-300 hover:-translate-y-0.5;
  min-height:48px;
}

</style> -->
