<template>
  <div class="bg-[#130C0E]">
    <!-- Navigation arrows -->
    <div class="hidden lg:block lg:ml-[340px] lg:pt-10">
      <!-- Chevron left -->
      <div
        class="mr-2 inline-block border-[2px] border-white rounded-full cursor-pointer"
        @click="showPrevSlide"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          height="24px"
          viewBox="0 0 24 24"
          width="24px"
          fill="#ffffff"
        >
          <path d="M0 0h24v24H0V0z" fill="none" />
          <path d="M15.41 7.41L14 6l-6 6 6 6 1.41-1.41L10.83 12l4.58-4.59z" />
        </svg>
      </div>

      <!-- Chevron right -->
      <div
        class="inline-block border-[2px] border-white rounded-full cursor-pointer"
        @click="showNextSlide"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          height="24px"
          viewBox="0 0 24 24"
          width="24px"
          fill="#ffffff"
        >
          <path d="M0 0h24v24H0V0z" fill="none" />
          <path d="M10 6L8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6-6-6z" />
        </svg>
      </div>
    </div>

    <div ref="swiper" v-swiper:mySwiper="swiperOption">
      <div class="swiper-wrapper">
        <!-- Slide 1 -->
        <div
          class="swiper-slide h-full px-5 sm:px-10 py-10 lg:py-20 flex flex-col-reverse sm:flex-row justify-center items-center gap-6"
        >
          <!-- Text -->
          <div>
            <h3 class="text-4xl text-orange uppercase font-bold">
              Verschiedene Toppings
            </h3>
            <p class="my-6 max-w-xs text-base text-white">
              Jeder Donut von uns besitzt sein ganz eigenes Topping. Wähle ganz
              einfach zwischen deinen lieblings Donut Toppings.
            </p>
          </div>

          <!-- Image -->
          <div>
            <div>
              <img
                class="max-w-xs"
                src="/img/schokoladen-donut-mit-streusel.png"
              />
            </div>
          </div>
        </div>

        <!-- Slide 2 -->
        <div
          class="swiper-slide bg-[#130C0E] h-full px-5 sm:px-10 py-10 lg:py-20 flex flex-col-reverse sm:flex-row justify-center items-center gap-6"
        >
          <!-- Text -->
          <div>
            <h3 class="text-4xl text-orange uppercase font-bold">
              Einzigartige Füllung
            </h3>
            <p class="my-6 max-w-xs text-base text-white">
              Wir entwickeln einzigartige Füllung speziell für jeden Geschmack.
              Wir sind sicher, auch du wirst unsere Füllungen lieben!
            </p>
          </div>

          <!-- Image -->
          <div>
            <div>
              <img
                class="max-w-xs"
                src="/img/schokoladen-donut-mit-streusel.png"
              />
            </div>
          </div>
        </div>

        <!-- Slide 3 -->
        <div
          class="swiper-slide bg-[#130C0E] h-full px-5 sm:px-10 py-10 lg:py-20 flex flex-col-reverse sm:flex-row justify-center items-center gap-6"
        >
          <!-- Text -->
          <div>
            <h3 class="text-4xl text-orange uppercase font-bold">
              Vegane Donuts
            </h3>
            <p class="my-6 max-w-xs text-base text-white">
              Wir sorgen dafür, dass auch du, ohne tierische Produkte, deine
              lieblings Donuts genießen kannst.
            </p>
          </div>

          <!-- Image -->
          <div>
            <div>
              <img
                class="max-w-xs"
                src="/img/schokoladen-donut-mit-streusel.png"
              />
            </div>
          </div>
        </div>
      </div>
      <div slot="pagination" class="swiper-pagination"></div>
    </div>
  </div>
</template>

<script>
import { directive } from 'vue-awesome-swiper'

export default {
  name: 'Slider',
  directives: {
    swiper: directive,
  },
  data() {
    return {
      swiperOption: {
        pagination: {
          el: '.swiper-pagination',
        },
      },
    }
  },
  computed: {
    swiper(vm) {
      return vm.$refs.swiper.swiper
    },
  },
  methods: {
    showNextSlide() {
      this.swiper.slideNext()
    },
    showPrevSlide() {
      this.swiper.slidePrev()
    },
  },
}
</script>
