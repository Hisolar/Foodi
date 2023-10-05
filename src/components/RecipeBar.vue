<template>
  <div class="bg-white shadow-md rounded-lg relative p-2">
    <img class="rounded-lg" :src="props.image" alt="" />
    <SButton
      variant="sublime"
      class="absolute top-4 right-4 flex gap-2 items-center"
    >
      <font-awesome-icon :icon="['fas', 'star']" style="color: #ff9500" />
      <p>{{ props.rating }}</p>
    </SButton>

    <div class="px-2 py-10 flex flex-col gap-4">
      <h1>{{ props.category }}</h1>
      <p class="text-xs">
        {{ props.description }}
      </p>
      <div class="bg-slate-5.000 w-full h-[1px] px-2"></div>
      <div class="flex items-center justify-between">
        <h1>$120.00</h1>
        <SButton variant="outline" class="text-xs">Add to Cart</SButton>
      </div>
    </div>
  </div>
</template>
<script setup>
import SButton from "./SButton.vue";

const props = defineProps({
  image: String,
  rating: Number,
  category: String,
  description: String,
});
</script>
