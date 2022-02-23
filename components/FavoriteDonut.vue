<template>
  <div>
    <div
      class="bg-white flex flex-row justify-center items-center h-80 sm:min-h-min"
    >
      <img :src="donutImg" />
    </div>
    <h5 class="mt-3 text-base text-gray font-bold">{{ donutName }}</h5>
    <div class="mb-14 text-base text-gray">{{ donutPrice }}</div>
  </div>
</template>

<script>
export default {
  props: {
    donutImg: {
      type: String,
      required: true,
    },
    donutName: {
      type: String,
      required: true,
    },
    donutPrice: {
      type: String,
      required: true,
    },
  },
}
</script>
