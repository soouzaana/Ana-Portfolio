<script setup>
import { defineAsyncComponent } from "vue";
import loadingSpinner from "@/components/loadingSpinner.vue";

const NavBar = defineAsyncComponent(() => import("@/components/NavBar.vue"));
const HeroSection = defineAsyncComponent(() =>
  import("@/components/HeroSection.vue")
);
</script>

<template>
  <div class="bg-[#111827] min-h-screen">
    <!-- wrap components in suspense to handle loading -->
    <Suspense>
      <template #default>
        <!-- wrap all components inside a single root element -->
        <div>
          <NavBar />
          <HeroSection />
        </div>
      </template>
      <template #fallback>
        <div class="flex justify-center items-center min-h-screen">
          <loadingSpinner />
        </div>
      </template>
    </Suspense>
  </div>
</template>

<style>
* {
  scrollbar-width: thin;
  scrollbar-color: #ec4899 #f1f1f1;
}
</style>
