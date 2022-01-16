<template>
  <div
    class="flex flex-row justify-center items-center px-8 py-3 rounded-full uppercase font-bold"
    :class="[
      {
        'bg-orange hover:bg-gray text-gray hover:text-orange': bgPrimary,
        'border border-gray bg-white hover:bg-gray text-gray hover:text-white':
          outlined,
        'bg-gray hover:bg-white text-white hover:text-gray': bgSecondary,
      },
    ]"
  >
    <!-- Pencil Icon -->
    <div v-if="showIcon && iconLeft && !iconRight" class="mr-2">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        height="24px"
        viewBox="0 0 24 24"
        width="24px"
        fill="#000000"
      >
        <path d="M0 0h24v24H0V0z" fill="none" />
        <path
          d="M14.06 9.02l.92.92L5.92 19H5v-.92l9.06-9.06M17.66 3c-.25 0-.51.1-.7.29l-1.83 1.83 3.75 3.75 1.83-1.83c.39-.39.39-1.02 0-1.41l-2.34-2.34c-.2-.2-.45-.29-.71-.29zm-3.6 3.19L3 17.25V21h3.75L17.81 9.94l-3.75-3.75z"
        />
      </svg>
    </div>

    <!-- Button Label -->
    <slot>Click me</slot>

    <!-- Play Icon -->
    <div v-if="showIcon && iconRight" class="ml-2">
      <svg
        class="fill-orange"
        xmlns="http://www.w3.org/2000/svg"
        height="24px"
        viewBox="0 0 24 24"
        width="24px"
        fill="#000000"
      >
        <path d="M0 0h24v24H0V0z" fill="none" />
        <path
          d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 14.5v-9l6 4.5-6 4.5z"
        />
      </svg>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    outlined: {
      type: Boolean,
      required: false,
    },
    showIcon: {
      type: Boolean,
      default: false,
      required: false,
    },
    iconLeft: {
      type: Boolean,
      default: true,
      required: false,
    },
    iconRight: {
      type: Boolean,
      default: false,
      required: false,
    },
    bgPrimary: {
      type: Boolean,
      default: false,
      required: false,
    },
    bgSecondary: {
      type: Boolean,
      default: false,
      required: false,
    },
    textColor: {
      type: String,
      default: 'gray',
      required: false,
    },
  },
}
</script>
