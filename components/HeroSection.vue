<template>
  <div class="bg-blue h-full px-5 py-10 lg:py-20">
    <div class="lg:flex lg:flex-row lg:justify-center lg:items-center">
      <!-- Heading -->
      <div class="uppercase text-white text-opacity-50">
        <h1 class="text-5xl lg:text-6xl font-bold lg:max-w-xs">
          Entdecke die Vielfalt.
        </h1>
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
    </div>

    <!-- CTA Buttons -->
    <div class="lg:mt-12 flex flex-row justify-center items-center gap-4">
      <!-- Classic -->
      <base-button class="mt-6" bg-primary>Classic</base-button>
      <!-- Fancy -->
      <base-button class="mt-6" bg-primary>Fancy</base-button>
    </div>
  </div>
</template>
