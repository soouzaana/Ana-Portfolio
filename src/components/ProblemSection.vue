<template>
  <section class="py-24 md:py-32 border-t border-[rgba(86,18,105,0.1)]">
    <div class="max-w-[120rem] mx-auto px-[4vw]">
      <!-- Título -->
      <div class="mb-16">
        <span class="text-xs font-semibold tracking-[3px] uppercase mb-4 block text-[#e2aef0]">
          O Problema
        </span>
        <h2
          class="font-extrabold text-3xl md:text-5xl leading-tight max-w-2xl text-[#561269] -tracking-[0.02em]"
        >
          Sua empresa está perdendo clientes enquanto você lê isso.
        </h2>
      </div>

      <!-- Grid de problemas -->
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-0">
        <!-- Item 1 -->
        <div
          class="p-8 md:p-10 border-t sm:border-t-0 border-l first:border-l-0 sm:first:border-l sm:[&:nth-child(1)]:border-l-0 sm:[&:nth-child(3)]:border-l-0 lg:[&:nth-child(3)]:border-l border-[rgba(86,18,105,0.1)]"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="lucide lucide-triangle-alert w-6 h-6 mb-6 text-[#e2aef0]"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path d="m21.73 18-8-14a2 2 0 0 0-3.48 0l-8 14A2 2 0 0 0 4 21h16a2 2 0 0 0 1.73-3" />
            <path d="M12 9v4" />
            <path d="M12 17h.01" />
          </svg>
          <h3 class="font-bold text-lg mb-3 text-[#561269]">Fuga de Valor</h3>
          <p class="text-base leading-relaxed text-[#561269]/60">
            Empresas que dependem apenas de redes sociais não são donas da sua audiência. Uma
            mudança de algoritmo pode eliminar sua visibilidade.
          </p>
        </div>

        <!-- Item 2 -->
        <div
          class="p-8 md:p-10 border-t sm:border-t-0 border-l first:border-l-0 sm:first:border-l sm:[&:nth-child(1)]:border-l-0 sm:[&:nth-child(3)]:border-l-0 lg:[&:nth-child(3)]:border-l border-[rgba(86,18,105,0.1)]"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="lucide lucide-gauge w-6 h-6 mb-6 text-[#e2aef0]"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path d="m12 14 4-4" />
            <path d="M3.34 19a10 10 0 1 1 17.32 0" />
          </svg>
          <h3 class="font-bold text-lg mb-3 text-[#561269]">Obsolescência</h3>
          <p class="text-base leading-relaxed text-[#561269]/60">
            Sites lentos e desatualizados afastam clientes de alto ticket em segundos. Cada segundo
            de delay reduz suas conversões em 7%.
          </p>
        </div>

        <!-- Item 3 -->
        <div
          class="p-8 md:p-10 border-t sm:border-t-0 border-l first:border-l-0 sm:first:border-l sm:[&:nth-child(1)]:border-l-0 sm:[&:nth-child(3)]:border-l-0 lg:[&:nth-child(3)]:border-l border-[rgba(86,18,105,0.1)]"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="lucide lucide-eye w-6 h-6 mb-6 text-[#e2aef0]"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path
              d="M2.062 12.348a1 1 0 0 1 0-.696 10.75 10.75 0 0 1 19.876 0 1 1 0 0 1 0 .696 10.75 10.75 0 0 1-19.876 0"
            />
            <circle cx="12" cy="12" r="3" />
          </svg>
          <h3 class="font-bold text-lg mb-3 text-[#561269]">Invisibilidade</h3>
          <p class="text-base leading-relaxed text-[#561269]/60">
            A falta de presença profissional no Google é uma barreira invisível para o seu
            crescimento e autoridade no mercado.
          </p>
        </div>

        <!-- Item 4 -->
        <div
          class="p-8 md:p-10 border-t sm:border-t-0 border-l first:border-l-0 sm:first:border-l sm:[&:nth-child(1)]:border-l-0 sm:[&:nth-child(3)]:border-l-0 lg:[&:nth-child(3)]:border-l border-[rgba(86,18,105,0.1)]"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="lucide lucide-puzzle w-6 h-6 mb-6 text-[#e2aef0]"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path
              d="M15.39 4.39a1 1 0 0 0 1.68-.474 2.5 2.5 0 1 1 3.014 3.015 1 1 0 0 0-.474 1.68l1.683 1.682a2.414 2.414 0 0 1 0 3.414L19.61 15.39a1 1 0 0 1-1.68-.474 2.5 2.5 0 1 0-3.014 3.015 1 1 0 0 1 .474 1.68l-1.683 1.682a2.414 2.414 0 0 1-3.414 0L8.61 19.61a1 1 0 0 0-1.68.474 2.5 2.5 0 1 1-3.014-3.015 1 1 0 0 0 .474-1.68l-1.683-1.682a2.414 2.414 0 0 1 0-3.414L4.39 8.61a1 1 0 0 1 1.68.474 2.5 2.5 0 1 0 3.014-3.015 1 1 0 0 1-.474-1.68l1.683-1.682a2.414 2.414 0 0 1 3.414 0z"
            />
          </svg>
          <h3 class="font-bold text-lg mb-3 text-[#561269]">Desordem Digital</h3>
          <p class="text-base leading-relaxed text-[#561269]/60">
            Sistemas que não conversam entre si geram custos operacionais, retrabalho e perda de
            oportunidades diárias.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// Nenhuma lógica JS necessária aqui
</script>
