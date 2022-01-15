<template>
  <div
    class="bg-white h-full px-5 py-10 lg:py-20 lg:flex lg:flex-row lg:justify-center lg:items-center lg:gap-8"
  >
    <!-- Text + CTA Button -->
    <div>
      <div class="text-gray text-center">
        <h2 class="uppercase font-bold text-4xl">
          Unsere Aktion!<br />
          3 für 2
        </h2>
        <div class="mt-6 normal-case">
          Entscheide dich für 3 Donuts und bezahle nur 2.
        </div>
      </div>
      <!-- CTA Button -->
      <div class="mt-6 flex justify-center">
        <base-button bg-color="white" outlined show-icon
          >Wähle deine Donuts</base-button
        >
      </div>
    </div>

    <!-- Donut variations Image -->
    <div class="hidden lg:block">
      <img
        class="max-w-2xl"
        src="/img/verschiedene-donut-variationen.png"
        alt="Donut Variationen"
      />
    </div>
  </div>
</template>
