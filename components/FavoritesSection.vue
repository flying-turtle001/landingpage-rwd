<template>
  <div class="bg-[#D9D9DB] h-full pl-5 lg:px-20 py-10 lg:py-20">
    <div class="lg:flex lg:flex-row lg:justify-between lg:items-center">
      <!-- Heading -->
      <h4 class="mb-6 text-gray font-bold uppercase text-3xl">
        Am beliebtesten
      </h4>

      <!-- Navigation arrows -->
      <div class="hidden lg:block lg:mr-14">
        <!-- Chevron left -->
        <div
          class="mr-2 inline-block border-[2px] border-gray rounded-full cursor-pointer"
          @click="showPrevSlide"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            height="24px"
            viewBox="0 0 24 24"
            width="24px"
            fill="#333132"
          >
            <path d="M0 0h24v24H0V0z" fill="none" />
            <path d="M15.41 7.41L14 6l-6 6 6 6 1.41-1.41L10.83 12l4.58-4.59z" />
          </svg>
        </div>

        <!-- Chevron right -->
        <div
          class="inline-block border-[2px] border-gray rounded-full cursor-pointer"
          @click="showNextSlide"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            height="24px"
            viewBox="0 0 24 24"
            width="24px"
            fill="#333132"
          >
            <path d="M0 0h24v24H0V0z" fill="none" />
            <path d="M10 6L8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6-6-6z" />
          </svg>
        </div>
      </div>
    </div>

    <!-- Slider - Mobil -->
    <div v-swiper:mySwiper="swiperOption" class="sm:hidden">
      <div class="swiper-wrapper">
        <!-- Donut 1 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/fancy-donut.png"
            donut-name="Cheesecake Donut"
            donut-price="7,99 €"
          />
        </div>

        <!-- Donut 2 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-schokoriegel-und-toffifee.png"
            donut-name="Toffi Donut"
            donut-price="6,99 €"
          />
        </div>

        <!-- Donut 3 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-weisser-schokolade-und-himbeere.png"
            donut-name="White Crispy Donut"
            donut-price="5,99 €"
          />
        </div>

        <!-- Donut 4 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-herz-streussel.png"
            donut-name="Fall in love Donut"
            donut-price="3,99 €"
          />
        </div>

        <!-- Donut 5 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-schokoriegel-und-fruechten.png"
            donut-name="Schoco Kiss Donut"
            donut-price="5,99 €"
          />
        </div>

        <!-- Donut 6 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-schokolade-und-fruechten.png"
            donut-name="Fruit Love Donut"
            donut-price="6,99 €"
          />
        </div>

        <!-- Donut 7 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/veganer-donut.png"
            donut-name="Vegan Star Donut"
            donut-price="6,99 €"
          />
        </div>

        <!-- Donut 8 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-maxi-king-und-fruechten.png"
            donut-name="Maxi King Donut"
            donut-price="6,99 €"
          />
        </div>
      </div>
      <div slot="pagination" class="swiper-pagination"></div>
    </div>

    <!-- Slider - Tablet / Desktop -->
    <div
      ref="swiper"
      v-swiper:mySwiperDesk="swiperOptionDesk"
      class="hidden sm:block"
    >
      <div class="swiper-wrapper cursor-pointer">
        <!-- Donut 1 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/fancy-donut.png"
            donut-name="Cheesecake Donut"
            donut-price="7,99 €"
          />
        </div>

        <!-- Donut 2 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-schokoriegel-und-toffifee.png"
            donut-name="Toffi Donut"
            donut-price="6,99 €"
          />
        </div>

        <!-- Donut 3 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-weisser-schokolade-und-himbeere.png"
            donut-name="White Crispy Donut"
            donut-price="5,99 €"
          />
        </div>

        <!-- Donut 4 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-herz-streussel.png"
            donut-name="Fall in love Donut"
            donut-price="3,99 €"
          />
        </div>

        <!-- Donut 5 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-schokoriegel-und-fruechten.png"
            donut-name="Schoco Kiss Donut"
            donut-price="5,99 €"
          />
        </div>

        <!-- Donut 6 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-schokolade-und-fruechten.png"
            donut-name="Fruit Love Donut"
            donut-price="6,99 €"
          />
        </div>

        <!-- Donut 7 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/veganer-donut.png"
            donut-name="Vegan Star Donut"
            donut-price="6,99 €"
          />
        </div>

        <!-- Donut 8 -->
        <div class="swiper-slide">
          <FavoriteDonut
            donut-img="/img/donut-mit-maxi-king-und-fruechten.png"
            donut-name="Maxi King Donut"
            donut-price="6,99 €"
          />
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
        slidesPerView: 'auto',
        spaceBetween: 15,
        pagination: {
          el: '.swiper-pagination',
          clickable: true,
        },
      },
      swiperOptionDesk: {
        slidesPerView: 4,
        spaceBetween: 30,
        slidesPerGroup: 4,
        loop: true,
        loopFillGroupWithBlank: true,
        pagination: {
          el: '.swiper-pagination',
          clickable: true,
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
