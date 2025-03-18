<script lang="ts" setup>
const props = defineProps({
  image: {
    type: String,
    required: true,
  },
  title: String,
  description: String,
});
</script>
<template>
  <div class="flex flex-col">
    <figure>
      <img :src="image" class="mb-7.5" :alt="title" />
      <div class="text-[21px] font-bold mb-2.5">{{ title }}</div>
      <p class="card-description max-w-[315px] mx-auto">
        {{ description }}
      </p>
    </figure>
  </div>
</template>

<style></style>
