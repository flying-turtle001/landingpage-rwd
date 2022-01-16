<template>
  <div
    id="classic-fancy-donut"
    class="bg-gray h-full px-5 py-10 lg:py-20 sm:flex sm:flex-row sm:justify-center sm:items-center sm:gap-16"
  >
    <!-- Classic Donut -->
    <div class="lg:mt-14 lg:max-w-md">
      <!-- Donut Image -->
      <div class="flex justify-center">
        <img
          class="max-w-xs sm:max-w-2xl"
          src="/img/classic-donut.png"
          alt=""
        />
      </div>

      <div class="text-center">
        <!-- Heading -->
        <h3 class="mt-6 text-xl text-orange font-bold uppercase">Classic</h3>
        <div class="text-xs text-white">Ab 4,99€</div>
        <!-- Link -->
        <NuxtLink
          to="/"
          class="inline-block mt-6 text-sm uppercase text-orange font-bold"
          >Alle ></NuxtLink
        >
        <!-- Description -->
        <p class="mt-6 text-white text-base">
          Der Classic Donut ist der König aller Donuts. Er überzeugt durch seine
          Eleganz und Geschmack und ist bei jedem Anlass die richtige Wahl. Mit
          dem Classic Donut bist Du immer richtig bedient und sorgst auf jeder
          Party für die richtige Stimmung.
        </p>
      </div>
    </div>

    <!-- Fancy Donut -->
    <div class="mt-10 lg:mt-0 lg:max-w-md">
      <!-- Donut Image -->
      <div class="flex justify-center">
        <img class="max-w-xs sm:max-w-2xl" src="/img/fancy-donut.png" alt="" />
      </div>
      <div class="text-center">
        <!-- Heading -->
        <h3 class="mt-6 text-xl text-orange font-bold uppercase">Fancy</h3>
        <div class="text-xs text-white">Ab 8,99€</div>
        <!-- Link -->
        <NuxtLink
          to="/"
          class="inline-block mt-6 text-sm uppercase text-orange font-bold"
          >Alle ></NuxtLink
        >
        <!-- Description -->
        <p class="mt-6 text-white text-base">
          Du möchtest deine Party aufpeppen, deine Freunde überraschen oder
          einfach mal was anderes ausprobieren? Kein Problem! Mit unseren
          aussergewöhnlichen Donuts findest auch Du bestimmt einen Donut, der
          alle überzeugen wird. Und das nicht nur mit seinem Geschmack!
        </p>
      </div>
    </div>
  </div>
</template>
