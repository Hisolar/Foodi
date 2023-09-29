<!-- <template>
  <button
    class="px-4 py-2 rounded-full"
    :style="{ backgroundColor: props.backgroundColor, color: props.textColor }"
  >
    <slot />
  </button>
</template>

<script setup>
const props = defineProps({
  backgroundColor: {
    type: String,
    default: "red",
  },

  textColor: {
    type: String,
  },
  //   vaiant: {
  //     type: String,
  //     default: Primary,
  //   },
});
</script> -->

<template>
  <button
    class="px-4 py-2"
    :class="
      props.variant == 'primary'
        ? 'bg-[#FE0103] rounded-full'
        : props.variant == 'outline'
        ? 'border border-white rounded-full'
        : props.variant == 'secondary'
        ? 'border border-[#FE0103] rounded-full'
        : ''
    "
  >
    <slot />
  </button>
</template>

<script setup>
const props = defineProps({
  variant: {
    type: String,
  },
});
</script>
