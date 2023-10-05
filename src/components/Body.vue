<template>
  <section class="container mx-auto px-6">
    <article class="grid gap-3 lg:grid-cols-2 pt-10 items-center relative">
      <div class="flex flex-col gap-5">
        <SButton variant="primary" class="flex items-center gap-2 max-w-fit">
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v16961435.070/foodi/quality_xnjnka.svg"
            alt=""
          />
          Qualityfull Food</SButton
        >
        <h1 class="text-5xl lg:text-[74px] font-bold font-display">
          Enjoy Your Delicious Food
        </h1>
        <p>
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry. Lorem Ipsum has been the industry's...
        </p>
        <div class="flex items-center gap-4 z-10">
          <SButton variant="tertiary">Order Now</SButton>

          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696144383/foodi/work_ache3e.svg"
            alt=""
          />
        </div>
      </div>
      <div class="flex flex-col gap-4">
        <img
          src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014129/foodi/banner_c3jt0s.svg"
          alt=""
        />

        <div class="grid grid-cols-3 gap-10">
          <div class="flex flex-col items-center gap-2">
            <h1 class="font-bold text-3xl">120K</h1>
            <p>Website Visitor</p>
          </div>
          <div class="flex flex-col items-center gap-2">
            <h1 class="font-bold text-3xl">65K</h1>
            <p>Use online order</p>
          </div>
          <div class="flex flex-col items-center gap-2">
            <h1 class="font-bold text-3xl">45K</h1>
            <p>5.0 star review</p>
          </div>
        </div>
      </div>
      <img
        class="absolute bottom-0 -left-10 z-0 hidden lg:block"
        src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014129/foodi/dot_bgm87y.svg"
        alt=""
      />
      <img
        class="absolute top-6 left-56 lg:left-80"
        src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014131/foodi/starG_zpnvsq.svg"
        alt=""
      />
      <img
        class="hidden lg:block lg:absolute lg:bottom-24 lg:right-1/2"
        src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014131/foodi/starB_w8gjbl.svg"
        alt=""
      />
    </article>
  </section>
</template>

<script setup>
import SButton from "./SButton.vue";
</script>
