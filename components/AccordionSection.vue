<template>
  <div class="h-full px-5 py-10 lg:py-20">
    <!-- Good to know - Tab -->
    <div
      class="flex flex-col justify-center items-center cursor-pointer"
      @click="firstTabIsOpen = !firstTabIsOpen"
    >
      <h5 class="text-xl font-bold text-gray uppercase">Gut zu wissen</h5>
      <div v-if="!firstTabIsOpen">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          height="24px"
          viewBox="0 0 24 24"
          width="24px"
          fill="#333132"
        >
          <path d="M0 0h24v24H0V0z" fill="none" />
          <path
            d="M13 7h-2v4H7v2h4v4h2v-4h4v-2h-4V7zm-1-5C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 8-8 8z"
          />
        </svg>
      </div>
      <div v-if="firstTabIsOpen">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          enable-background="new 0 0 24 24"
          height="24px"
          viewBox="0 0 24 24"
          width="24px"
          fill="#333132"
        >
          <g><rect fill="none" height="24" width="24" /></g>
          <g>
            <g>
              <path
                d="M7,11v2h10v-2H7z M12,2C6.48,2,2,6.48,2,12s4.48,10,10,10s10-4.48,10-10S17.52,2,12,2z M12,20c-4.41,0-8-3.59-8-8 s3.59-8,8-8s8,3.59,8,8S16.41,20,12,20z"
              />
            </g>
          </g>
        </svg>
      </div>
    </div>
    <!-- Content -->
    <div
      v-if="firstTabIsOpen"
      class="sm:grid sm:grid-cols-3 sm:gap-12 lg:gap-12 sm:px-10 lg:px-20"
    >
      <!-- Average donut size -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Größe</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">Ø 8,5 cm</span>
      </div>

      <!-- Weight -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Gewicht</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">ca. 100 g</span>
      </div>

      <!-- Calorie -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Kalorien</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">452</span>
      </div>

      <!-- Fat content -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Fettgehalt</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">25 g</span>
      </div>

      <!-- Protein -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Protein</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">4,9 g</span>
      </div>
    </div>

    <!-- Divider -->
    <div class="my-6 mx-auto w-3/4 h-[1px] bg-gray"></div>

    <!-- Ingredients - Tab -->
    <div
      class="flex flex-col justify-center items-center cursor-pointer"
      @click="secondTabIsOpen = !secondTabIsOpen"
    >
      <h5 class="text-xl font-bold text-gray uppercase">Zutaten</h5>
      <div v-if="!secondTabIsOpen">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          height="24px"
          viewBox="0 0 24 24"
          width="24px"
          fill="#333132"
        >
          <path d="M0 0h24v24H0V0z" fill="none" />
          <path
            d="M13 7h-2v4H7v2h4v4h2v-4h4v-2h-4V7zm-1-5C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 8-8 8z"
          />
        </svg>
      </div>
      <div v-if="secondTabIsOpen">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          enable-background="new 0 0 24 24"
          height="24px"
          viewBox="0 0 24 24"
          width="24px"
          fill="#333132"
        >
          <g><rect fill="none" height="24" width="24" /></g>
          <g>
            <g>
              <path
                d="M7,11v2h10v-2H7z M12,2C6.48,2,2,6.48,2,12s4.48,10,10,10s10-4.48,10-10S17.52,2,12,2z M12,20c-4.41,0-8-3.59-8-8 s3.59-8,8-8s8,3.59,8,8S16.41,20,12,20z"
              />
            </g>
          </g>
        </svg>
      </div>
    </div>

    <!-- Content -->
    <div
      v-if="secondTabIsOpen"
      class="sm:grid sm:grid-cols-3 sm:gap-12 lg:gap-12 sm:px-10 lg:px-20"
    >
      <!-- Wheat flour -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Weizenmehl</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">500 g</span>
      </div>

      <!-- Milk -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Milch</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">200 g</span>
      </div>

      <!-- Yeast -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Hefe</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">30 g</span>
      </div>

      <!-- Butter -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Butter</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">60 g</span>
      </div>

      <!-- Sugar -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Zucker</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">50 g</span>
      </div>

      <!-- Eggs -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Eier</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">1</span>
      </div>

      <!-- Salt -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Salz</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">5 g</span>
      </div>

      <!-- Vanilla flavoring -->
      <div class="my-4">
        <h6 class="text-gray font-bold text-base uppercase">Vanillearoma</h6>
        <div class="mb-4 mx-auto w-full h-[1.5px] bg-gray"></div>
        <span class="text-gray font-bold text-5xl">1 TL</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      firstTabIsOpen: false,
      secondTabIsOpen: false,
    }
  },
}
</script>
