<script lang="ts" setup>
import Card from "@/components/Card.vue";
import cardBlock1 from "@/assets/img/card-block-1.png";
import cardBlock2 from "@/assets/img/card-block-2.png";
import cardBlock3 from "@/assets/img/card-block-3.png";

const cards = [
  {
    title: "RED",
    image: cardBlock1,
    description: "Red foods remind us of berries and soft fruits, so we anticipate a sweet taste.",
  },
  {
    title: "Green",
    image: cardBlock2,
    description:
      "Fresh, zingy green colours are reminiscent of unripe fruit, promising sour or acid flavours",
  },
  {
    title: "White",
    image: cardBlock3,
    description:
      "White foods evoke memories of salt and salty flavours, driving the expectation of a savoury treat.",
  },
];
</script>
<template>
  <div class="container md:max-w-[1146px] mx-auto py-20 text-center space-y-[30px]">
    <h3 class="section-title w-auto mx-auto inline-block">Taste the Colours</h3>
    <div class="flex gap-2.5">
      <card v-for="(card, index) in cards" v-bind="card" :key="index" class="flex-1" />
    </div>
  </div>
</template>

<style></style>
