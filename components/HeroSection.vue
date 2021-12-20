<template>
  <div class="bg-blue h-full px-5 py-10">
    <div class="uppercase text-white text-opacity-50">
      <h1 class="text-5xl font-bold">Entdecke die Vielfalt.</h1>
      <span class="text-base">Für jeden Anlass</span>
      <br />
      <span
        class="inline-block mt-6 normal-case text-orange text-base font-bold"
        >Ab 4,99€</span
      >
    </div>

    <!-- Donut Image -->
    <div class="flex justify-center">
      <img
        class="max-w-xs"
        src="/img/schokoladen-donut-mit-streusel.png"
        alt=""
      />
    </div>

    <!-- CTA Buttons -->
    <div class="flex flex-row justify-center items-center gap-4">
      <!-- Classic -->
      <base-button class="mt-6">Classic</base-button>
      <!-- Fancy -->
      <base-button class="mt-6">Fancy</base-button>
    </div>
  </div>
</template>
