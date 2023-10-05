<template>
  <section class="bg-[#FDF2DD] w-full py-10">
    <article class="container mx-auto px-6">
      <div
        class="grid grid-cols-1 lg:grid-cols-2 gap-7 place-content-center items-center"
      >
        <div>
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014163/foodi/subscribe_bcna4y.svg"
            alt=""
          />
        </div>

        <div class="flex flex-col gap-5">
          <h1 class="text-5xl">Subscribe for Get update every New Offers</h1>
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the industry's standard dummy text.
          </p>
          <label>
            <input
              class="w-full py-3 px-5 rounded-full text-xs"
              type="email"
              placeholder="Enter your email adderss"
            />
          </label>
          <SButton variant="tertiary" class="max-w-fit text-xs">
            Subsribe Now</SButton
          >
        </div>
      </div>
    </article>
  </section>
</template>

<script setup>
import SButton from "./SButton.vue";
</script>
