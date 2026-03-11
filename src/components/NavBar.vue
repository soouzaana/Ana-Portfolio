<template>
  <nav
    :class="[
      'fixed top-0 left-0 right-0 z-50 transition-all duration-500 py-4 px-[4vw]',
      scrolled
        ? 'bg-white/95 backdrop-blur-[20px] border-b border-[rgba(86,18,105,0.08)]'
        : 'bg-transparent border-none',
    ]"
  >
    <div class="max-w-[120rem] mx-auto flex justify-between items-center">
      <!-- Logo -->
      <a
        href="#"
        :class="[
          'font-extrabold text-sm uppercase tracking-[2px] transition-colors duration-500 mr-4',
          scrolled ? 'text-primary' : 'text-primary',
        ]"
      >
        <!-- Logo texto -->
        <Logo class="logo-text" />

        <!-- Logo imagem -->
        <LogoImagem class="logo-img" />
      </a>

      <!-- Desktop Menu -->
      <div class="hidden md:flex items-center gap-8">
        <a
          href="#servicos"
          :class="[
            'text-xs font-semibold uppercase tracking-[1.5px] transition-colors duration-300',
            scrolled
              ? 'text-primary hover:text-secondary/50'
              : 'text-[#561269] hover:text-[#e2aef0]',
          ]"
        >
          Serviços
        </a>

        <a
          href="#portfolio"
          :class="[
            'text-xs font-semibold uppercase tracking-[1.5px] transition-colors duration-300',
            scrolled
              ? 'text-primary hover:text-secondary/50'
              : 'text-[#561269] hover:text-[#e2aef0]',
          ]"
        >
          Portfólio
        </a>

        <a
          href="#processo"
          :class="[
            'text-xs font-semibold uppercase tracking-[1.5px] transition-colors duration-300',
            scrolled
              ? 'text-primary hover:text-secondary/50'
              : 'text-[#561269] hover:text-[#e2aef0]',
          ]"
        >
          Processo
        </a>

        <a
          href="#contato"
          :class="[
            'text-xs font-semibold uppercase tracking-[1.5px] transition-colors duration-300',
            scrolled
              ? 'text-primary hover:text-secondary/50'
              : 'text-[#561269] hover:text-[#e2aef0]',
          ]"
        >
          Contato
        </a>

        <a
          href="#contato"
          class="px-6 py-3 text-xs font-semibold uppercase tracking-[1.5px] text-white bg-primary transition-all duration-300 hover:-translate-y-0.5 min-h-[48px]"
        >
          Falar Comigo
        </a>
      </div>

      <!-- Mobile Menu Button -->
      <button class="md:hidden p-2 text-primary" @click="toggleMenu" aria-label="Menu">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="w-6 h-6"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <line x1="4" x2="20" y1="12" y2="12" />
          <line x1="4" x2="20" y1="6" y2="6" />
          <line x1="4" x2="20" y1="18" y2="18" />
        </svg>
      </button>
    </div>
  </nav>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'
import Logo from './icons/logoName.vue'
import LogoImagem from './icons/logoImagem.vue'

const scrolled = ref(false)
const menuOpen = ref(false)

function toggleMenu() {
  menuOpen.value = !menuOpen.value
}

// Detecta scroll
function handleScroll() {
  scrolled.value = window.scrollY > 500
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

<style scoped>
/* Por padrão: mobile */
.logo-text {
  display: none;  /* não aparece no mobile */
}

.logo-img {
  display: block; /* aparece no mobile */
}

/* A partir de 768px (desktop) */
@media (min-width: 400px) {
  .logo-text {
    display: block;  /* mostra o texto no desktop */
  }
  .logo-img {
    display: none;   /* esconde a imagem no desktop */
  }
}
</style>
