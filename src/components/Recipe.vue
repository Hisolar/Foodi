<template>
  <section class="container mx-auto px-6">
    <article>
      <div class="flex flex-col items-center gap-3 text-center">
        <h1 class="text-3xl lg:text-5.0xl">Our Popular Recopies</h1>
        <p class="lg:w-1/2 max-w-max">
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry. Lorem Ipsum has been the industry's...
        </p>
      </div>

      <div
        class="flex items-center justify-center lg:justify-between flex-wrap gap-3 my-3"
      >
        <SButton
          class="my-3"
          @click="change_category(category)"
          v-for="(category, index) in refined_food_categories"
          :key="index"
          :variant="category.is_active ? 'primary' : 'outline'"
          >{{ category.name }}</SButton
        >
      </div>

      <div
        class="grid grid-cols-1 lg:grid-cols-3 gap-8 lg:gap-24 items-center justify-between"
      >
        <RecipeBar
          v-for="(recipe, index) in filtered_foods"
          :key="index"
          :image="recipe.image"
          :category="recipe.category.name"
          :rating="recipe.rating"
          :description="recipe.description"
        >
        </RecipeBar>
      </div>
      <div class="flex flex-col items-center my-6">
        <SButton variant="tertiary">
          <router-link to="more_foods">See more Foods</router-link></SButton
        >
        <p class="hidden">hello</p>
      </div>
    </article>
  </section>
</template>
<script setup>
import SButton from "./SButton.vue";
import RecipeBar from "./RecipeBar.vue";
import foods from "../data/foods";
import { ref, computed } from "vue";

const food_categories = [
  {
    id: "fast_foods",
    name: "Fast Foods",
  },

  {
    id: "breakfast_foods",
    name: "BreakFast Foods",
  },

  {
    id: "lunch_foods",
    name: "Lunch Foods",
  },

  {
    id: "drink_foods",
    name: "Drink Foods",
  },

  {
    id: "healthy_foods",
    name: "Healthy Foods",
  },

  {
    id: "special_foods",
    name: "Special Foods",
  },

  {
    id: "more_foods",
    name: "More Foods",
  },
];

const active_category_id = ref("fast_foods");

const filtered_foods = computed(() => {
  return foods.filter((food) => {
    return food.category.id == active_category_id.value;
  });
});

const refined_food_categories = computed(() => {
  return food_categories.map((category) => {
    const new_category = {};
    let selected_condition = false;

    if (category.id == active_category_id.value) {
      selected_condition = true;
    }

    return { ...category, is_active: selected_condition };
  });
});

const change_category = (category) => {
  active_category_id.value = category.id;
};
</script>
