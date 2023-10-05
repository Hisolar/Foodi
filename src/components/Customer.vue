<template>
  <section class="container mx-auto px-6">
    <div class="grid grid-cols-1 lg:grid-cols-2 gap-5 mt-12 lg:mt-24 pb-20">
      <div class="flex flex-col gap-3 relative">
        <h1 class="text-3xl lg:text-6xl">What Customer <br />Say Us</h1>
        <p>
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry. Lorem Ipsum has been the industry's standard.
        </p>
        <SButton variant="primary" class="max-w-fit"
          >Give your Valuable Feedback</SButton
        >
        <p class="text-xs">See All Feedback</p>
        <img
          class="absolute left-5 lg:left-48"
          src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696291354/man_ffqqra.svg"
          alt=""
        />
      </div>

      <div class="relative shadow-lg bg-white p-6">
        <div class="relative z-10 flex flex-col items-center gap-4">
          <div></div>
          <div class="flex gap-3 p-4">
            <img
              class=""
              src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696291353/quote_l1yz1q.svg"
              alt=""
            />
            <p class="">
              Lorem Ipsum is simply dummy text of the printing and typesetting
              industry. Lorem Ipsum has been the industry's standard dummy text.
            </p>
          </div>
          <div class="flex items-center gap-4">
            <img
              src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696294180/man_izegcb.svg"
              alt=""
            />
            <div>
              <h1>Albert Flores</h1>
              <p class="text-xs">albert.cruz@example.com</p>
            </div>
          </div>
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696291353/load_cvlvpn.svg"
            alt=""
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import SButton from "./SButton.vue";
</script>
<style></style>
