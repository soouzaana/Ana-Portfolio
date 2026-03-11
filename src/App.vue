<script setup>
import { defineAsyncComponent } from 'vue'
import loadingSpinner from '@/components/loadingSpinner.vue'

const NavBar = defineAsyncComponent(() => import('@/components/NavBar.vue'))
const HeroSection = defineAsyncComponent(() => import('@/components/HeroSection.vue'))
const ProblemSection = defineAsyncComponent(() => import('@/components/ProblemSection.vue'))
</script>

<template>
  <div class="bg-white min-h-screen">
    <!-- wrap components in suspense to handle loading -->
    <NavBar class="absolute top-0 left-0 w-full z-20" />
    <Suspense>
      <template #default>
        <HeroSection />
      </template>
      <template #fallback>
        <div class="flex justify-center items-center h-screen">
          <loadingSpinner />
        </div>
      </template>
    </Suspense>

    <ProblemSection />
  </div>
</template>

<style>
* {
  scrollbar-width: thin;
  scrollbar-color: #ec4899 #f1f1f1;
}

html,
body {
  margin: 0;
  padding: 0;
  height: 100%;
}
</style>
