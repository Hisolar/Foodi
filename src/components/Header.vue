<template>
  <section class="container mx-auto px-6">
    <div class="block lg:flex items-center justify-between pt-6">
      <div class="flex items-center justify-between">
        <img
          src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014129/foodi/logo_j1tgaz.svg"
          alt=""
        />
        <font-awesome-icon
          :icon="['fas', 'bars']"
          class="block lg:hidden text-2xl"
          @click="mobileToggle = !mobileToggle"
        />
      </div>

      <ul
        :class="
          mobileToggle ? 'block' : 'hidden lg:flex transition-all duration-500'
        "
        class="lg:items-center lg:gap-10"
      >
        <li class="mt-4">Home</li>
        <li class="mt-4">About</li>
        <li class="mt-4">Service</li>
        <li class="mt-4">Menu</li>
        <li class="mt-4">Contact</li>
      </ul>
      <ul class="hidden lg:flex lg:items-center lg:gap-10">
        <li>
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014129/foodi/search_mp5j9d.svg"
            alt=""
          />
        </li>
        <li class="flex items-center gap-2">
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014126/foodi/cart_h7pg6j.svg"
            alt=""
          />
          Cart
        </li>
        <li class="flex items-center gap-2">
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014131/foodi/signIn_wkfara.svg"
            alt=""
          />
          Sign In
        </li>
      </ul>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";
const mobileToggle = ref(false);
</script>
