<template>
  <article class="container mx-auto px-6">
    <div class="grid lg:grid-cols-2 lg:gap-10 my-10">
      <div class="flex flex-col gap-5 mt-14">
        <h1 class="text-4xl lg:text-5xl">What's Special About this Website?</h1>
        <p>
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry.
        </p>
        <p>
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry. Lorem Ipsum has been the industry's standard dummy text ever
          since.
        </p>
        <SButton variant="outline" class="max-w-fit">Read More</SButton>
      </div>
      <div class="grid lg:grid-cols-2 items-center gap-5 mt-5 lg:gap-5">
        <div class="flex items-center gap-2">
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014129/foodi/easyOrder_bflyit.svg"
            alt=""
          />
          <div>
            <h1 class="font-bold">Easy to order</h1>
            <p class="w-fill text-xs">
              Lorem Ipsum is simply dummy text of the printing
            </p>
          </div>
        </div>
        <div class="flex items-center gap-2">
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014126/foodi/homeDelivery_m3bahf.svg"
            alt=""
          />
          <div>
            <h1 class="font-bold">Home delivery</h1>
            <p class="w-fill text-xs">
              Lorem Ipsum is simply dummy text of the printing
            </p>
          </div>
        </div>
        <div class="flex items-center gap-2">
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014129/foodi/fatestDelivery_jikzxn.svg"
            alt=""
          />
          <div>
            <h1 class="font-bold">Fasted delivery</h1>
            <p class="w-fill text-xs">
              Lorem Ipsum is simply dummy text of the printing
            </p>
          </div>
        </div>
        <div class="flex items-center gap-2">
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014126/foodi/248_l6yi3n.svg"
            alt=""
          />
          <div>
            <h1 class="font-bold">24/8 delivery</h1>
            <p class="w-fill text-xs">
              Lorem Ipsum is simply dummy text of the printing
            </p>
          </div>
        </div>
        <div class="flex items-center gap-2">
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014126/foodi/bestQuality_enpc2n.svg"
            alt=""
          />
          <div>
            <h1 class="font-bold">Best quality</h1>
            <p class="w-fill text-xs">
              Lorem Ipsum is simply dummy text of the printing
            </p>
          </div>
        </div>
        <div class="flex items-center gap-2">
          <img
            src="https://res.cloudinary.com/dxiflsxek/image/upload/v1696014131/foodi/supperOffer_oiqusb.svg"
            alt=""
          />
          <div>
            <h1 class="font-bold">Supper offer</h1>
            <p class="w-fill text-xs">
              Lorem Ipsum is simply dummy text of the printing
            </p>
          </div>
        </div>
      </div>
    </div>
  </article>
</template>

<script setup>
import SButton from "./SButton.vue";
</script>
