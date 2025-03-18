<script lang="ts" setup>
 defineProps({
  image: {
    type: String,
    required: true,
  },
  title: String,
  description: String,
});
</script>
<template>
  <div class="flex flex-col max-sm:flex-col max-md:flex-row">
    <figure class="flex-1">
      <img :src="image" class="mb-7.5 w-full" :alt="title" />
    </figure>
    <div class="max-sm:p-0 max-md:p-4 max-sm:text-center max-md:text-left">
      <div class="text-[21px] font-bold mb-2.5">{{ title }}</div>
      <p class="card-description max-w-[315px] mx-auto">
        {{ description }}
      </p>
    </div>
  </div>
</template>

<style></style>
