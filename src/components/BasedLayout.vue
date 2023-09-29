<template>
  <div class="container mx-auto px-3">
    <div class="flex items-center justify-between">
      <slot name="logo"></slot>
      <ul class="flex items-center gap-10">
        <slot name="header"></slot>
      </ul>
      <ul class="flex items-center gap-10">
        <slot name="icon"></slot>
      </ul>
    </div>
    <div class="flex flex-col gap-6">
      <slot name="main"></slot>
      <div class="flex items-center justify-between"></div>
    </div>
    <div class="grid grid-cols-3 items-center place-content-between">
      <slot name="footer"></slot>
    </div>
  </div>
</template>

<script setup>
// const props = defineProps({
//   header: {
//     type: String,
//   },
// });
</script>
