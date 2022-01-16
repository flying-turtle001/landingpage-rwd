<template>
  <div class="relative overflow-hidden">
    <!-- Donut Video - Mobil -->
    <video class="sm:hidden absolute top-0 left-0 z-0" autoplay muted loop>
      <source src="/videos/donut-video-mobil.mp4" type="video/mp4" />
    </video>

    <!-- Donut Video - Tablet / Desktop -->
    <video
      class="hidden sm:block absolute top-0 left-0 z-0"
      autoplay
      muted
      loop
    >
      <source
        src="/videos/donuts-with-chocolate-and-cookies.mp4"
        type="video/mp4"
      />
    </video>

    <!-- Content -->
    <div
      class="relative h-[34rem] sm:h-[23rem] lg:h-[34rem] px-5 text-center flex flex-col justify-center items-center bg-black bg-opacity-50 z-50"
    >
      <h2 class="text-3xl text-white uppercase font-bold">
        Nicht nur essen. Genießen.
      </h2>
      <div class="mt-6">
        <base-button
          class="cursor-pointer"
          bg-color="gray"
          text-color="white"
          show-icon
          icon-right
          bg-secondary
          >Video abspielen</base-button
        >
      </div>
    </div>
  </div>
</template>
