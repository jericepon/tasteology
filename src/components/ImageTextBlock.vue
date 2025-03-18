<script lang="ts" setup>
import imageTextBlock1 from "@/assets/img/image-text-block-1.png";
import imageTextBlock2 from "@/assets/img/image-text-block-2.png";
import imageTextBlock3 from "@/assets/img/image-text-block-3.png";

let images = [
  { image: imageTextBlock1, class: "row-span-2" },
  { image: imageTextBlock2, class: "" },
  { image: imageTextBlock3, class: "" },
];
</script>
<template>
  <section>
    <div class="container md:max-w-[1146px] mx-auto py-20">
      <div class="flex flex-row gap-[30px]">
        <div class="grid grid-cols-2 gap-2.5">
          <figure :class="item.class" v-for="item in images" :key="item">
            <img :src="item.image" alt="" />
          </figure>
        </div>
        <article class="md:max-w-[362px] space-y-[30px]">
          <h3 class="section-title">WHAT DOES COOKING MEAN?</h3>
          <p class="card-description text-ellipsis line-clamp-11">
            Is it simply applying heat to a food product? A way of making certain food safe to eat?
            Or a way to create flavour and make food more appealing? This is just part of what Hervé
            This, the father of molecular gastronomy, has dedicated his life to finding out. We
            spoke to him to find out what his experiments have told him. And in the process even
            discovered the secret to cooking the perfect egg. Is it simply applying heat to a food
            product? A way of making certain food safe to eat? Or a way to create flavour and make
            food more appealing? This is just part of what Hervé This, the father of molecular
            gastronomy, has dedicated his life to finding out. We spoke to him to find out what his
            experiments have told him. And in the process even discovered the secret to cooking the
            perfect egg
          </p>
          <div class="flex flex-col space-y-2.5">
            <span class="text-[#cf1430] font-bold text-[15px] leading-[21px]">THE PERFECT EGG</span>
            <p class="font-bold text-[21px] leading-7.5">
              Keep water between 67 and 68°C for a flavourful, tender yolk
            </p>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>

<style></style>
