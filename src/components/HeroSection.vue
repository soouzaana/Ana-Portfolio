<template>
  <section class="relative min-h-screen flex items-center overflow-hidden">
    <!-- VIDEO BACKGROUND -->
    <video
      autoplay
      muted
      loop
      playsinline
      class="absolute inset-0 w-full h-full object-cover object-[center_0%]"
    >
      <source src="../../public/assets/video2.mp4" type="video/mp4" />
    </video>

    <!-- OVERLAY ROXO -->
    <div
      class="absolute inset-0"
      style="
        background: linear-gradient(
          90deg,
          rgba(20, 5, 30, 0.95) 0%,
          rgba(30, 8, 45, 0.9) 35%,
          rgba(45, 12, 70, 0.65) 60%,
          rgba(45, 12, 70, 0.35) 100%
        );
      "
    ></div>

    <!-- CONTEÚDO -->
    <div
      class="mt-20 w-full max-w-[120rem] mx-auto px-[4vw] grid grid-cols-1 lg:grid-cols-12 items-center relative z-10"
    >
      <!-- TEXTO -->
      <div class="lg:col-span-7 pt-32 pb-16 lg:py-0 text-white">
        <div class="mb-6">
          <span
            class="inline-block text-xs font-semibold tracking-[3px] uppercase px-4 py-2 border border-white/30 text-white"
          >
            Desenvolvedora Web Independente
          </span>
        </div>

        <h1
          class="font-extrabold leading-[0.88] tracking-tight mb-8"
          style="font-size: clamp(3rem, 7.5vw, 6.5rem); letter-spacing: -0.03em"
        >
          Arquitetando <br />
          Presença Digital <br />
          <span class="text-secondary">de Alto Nível.</span>
        </h1>

        <p class="text-lg md:text-xl max-w-lg mb-10 leading-relaxed text-white/80">
          Especialista em soluções web para negócios que exigem sofisticação, performance técnica e
          resultados estratégicos.
        </p>

        <div class="flex flex-wrap gap-4">
          <a
            href="#contato"
            class="inline-flex items-center gap-3 px-10 py-5 text-white font-semibold text-sm uppercase tracking-wider transition-all duration-500 hover:-translate-y-1 hover:shadow-2xl bg-primary"
          >
            Solicitar orçamento
          </a>

          <a
            href="#servicos"
            class="inline-flex items-center gap-3 px-10 py-5 font-semibold text-sm uppercase tracking-wider border border-white text-white transition-all duration-500 hover:-translate-y-1"
          >
            Ver serviços
          </a>
        </div>
      </div>
    </div>

    <div class="absolute bottom-0 left-0 right-0 h-px bg-white/20"></div>
  </section>
</template>

<style scoped>
video {
  filter: brightness(0.8) contrast(0.9);
}
</style>
