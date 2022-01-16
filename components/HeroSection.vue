<template>
  <div
    class="relative bg-gradient-radial from-[#205baf] via-[#0e2b5b] to-[#061131] h-full lg:h-[600px] px-5 py-10 sm:py-44 lg:py-20"
  >
    <!-- Heading -->
    <div
      class="lg:absolute lg:top-1/2 lg:left-1/2 lg:-translate-y-1/2 lg:-translate-x-[480px] uppercase text-white text-opacity-50"
    >
      <h1
        class="text-5xl sm:text-5xl lg:text-6xl font-bold sm:max-w-[200px] lg:max-w-[200px]"
      >
        Erlebe die Vielfalt.
      </h1>
      <span class="text-base">Für jeden Anlass</span>
      <br />
      <span
        class="inline-block mt-6 normal-case text-orange text-base font-bold"
        >Ab 2,99€</span
      >
    </div>

    <!-- Donut Image -->
    <div
      class="cursor-pointer w-full inline-block sm:max-w-xs sm:absolute sm:top-1/2 sm:left-1/2 sm:-translate-y-1/2 sm:-translate-x-1/2"
    >
      <!-- Product Spinner -->
      <VueProductSpinner :images="imgs"></VueProductSpinner>
      <img class="mx-auto mt-4 w-11" src="/icons/icon-360-degree.svg" alt="" />
    </div>

    <!-- CTA Buttons -->
    <div
      class="sm:absolute sm:bottom-0 lg:bottom-0 sm:left-1/2 lg:left-1/2 sm:-translate-y-1/2 lg:-translate-y-1/2 sm:-translate-x-1/2 lg:-translate-x-1/2 flex flex-row justify-center items-center gap-4"
    >
      <!-- Classic -->
      <base-button
        v-scroll-to="'#classic-fancy-donut'"
        class="mt-6 cursor-pointer"
        bg-primary
        >Classic</base-button
      >
      <!-- Fancy -->
      <base-button
        v-scroll-to="'#classic-fancy-donut'"
        class="mt-6 cursor-pointer"
        bg-primary
        >Fancy</base-button
      >
    </div>
  </div>
</template>

<script>
import VueProductSpinner from 'vue-product-spinner'

export default {
  components: {
    VueProductSpinner,
  },
  data() {
    return {
      imgs: [
        '/img/hero-donut/donut_14.png',
        '/img/hero-donut/donut_13.png',
        '/img/hero-donut/donut_12.png',
        '/img/hero-donut/donut_11.png',
        '/img/hero-donut/donut_10.png',
        '/img/hero-donut/donut_9.png',
        '/img/hero-donut/donut_8.png',
        '/img/hero-donut/donut_7.png',
        '/img/hero-donut/donut_6.png',
        '/img/hero-donut/donut_5.png',
        '/img/hero-donut/donut_4.png',
        '/img/hero-donut/donut_3.png',
        '/img/hero-donut/donut_2.png',
        '/img/hero-donut/donut_1.png',
      ],
    }
  },
}
</script>
