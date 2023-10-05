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
    class="px-4 py-1.5"
    :class="
      props.variant == 'primary'
        ? 'bg-[#F2BD57] rounded-full'
        : props.variant == 'outline'
        ? 'border border-[#F2BD57] rounded-full'
        : props.variant == 'secondary'
        ? 'border border-[#F2BD57] rounded-full'
        : props.variant == 'tertiary'
        ? 'bg-[#F2BD57] border-[2px] border-white rounded-full shadow-lg'
        : props.variant == 'sublime'
        ? 'bg-white rounded-full'
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
