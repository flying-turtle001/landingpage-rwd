<template>
  <div
    class="relative bg-gradient-radial from-[#205baf] via-[#0e2b5b] to-[#061131] h-full lg:h-[600px] px-5 py-10 lg:py-20"
  >
    <!-- Heading -->
    <div
      class="lg:absolute lg:top-1/2 lg:left-1/2 lg:-translate-y-1/2 lg:-translate-x-[520px] uppercase text-white text-opacity-50"
    >
      <h1 class="text-5xl lg:text-6xl font-bold lg:max-w-xs">
        Erlebe die Vielfalt.
      </h1>
      <span class="text-base">Für jeden Anlass</span>
      <br />
      <span
        class="inline-block mt-6 normal-case text-orange text-base font-bold"
        >Ab 4,99€</span
      >
    </div>

    <!-- Donut Image -->
    <div
      class="w-full inline-block lg:max-w-sm lg:absolute lg:top-1/2 lg:left-1/2 lg:-translate-y-1/2 lg:-translate-x-1/2"
    >
      <img src="/img/schokoladen-donut-mit-streusel.png" alt="" />
    </div>

    <!-- CTA Buttons -->
    <div
      class="lg:absolute lg:bottom-0 lg:left-1/2 lg:-translate-y-1/2 lg:-translate-x-1/2 flex flex-row justify-center items-center gap-4"
    >
      <!-- Classic -->
      <base-button class="mt-6" bg-primary>Classic</base-button>
      <!-- Fancy -->
      <base-button class="mt-6" bg-primary>Fancy</base-button>
    </div>
  </div>
</template>
