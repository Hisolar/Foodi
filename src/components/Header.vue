<template>
  <section class="container mx-auto px-6">
    <div>
      <!-- {{ logo }} -->
      <img src="../assets/logo.vue" alt="" />

      <ul class="flex items-center gap-10">
        <li>Home</li>
        <li>About</li>
        <li>Service</li>
        <li>Menu</li>
        <li>Contact</li>
      </ul>
      <ul>
        <li>
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1695897794/hobbie/search_swmtjk.svg"
            alt=""
          />
        </li>
        <li><img :src="notification" alt="" /></li>
        <li></li>
      </ul>
    </div>
  </section>
</template>

<script setup></script>
