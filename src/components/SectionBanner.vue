<script setup lang="ts">

defineProps({
  imgUrl: {
    type: String,
    required: true,
  },
  imgAltText: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <section class="relative w-full h-[50vh] flex flex-col justify-center items-center text-center text-white">
    <img :src="imgUrl" :alt="imgAltText" class="absolute inset-0 w-full h-full object-cover"/>

    <div class="frosted-glass relative z-10 w-full h-full flex flex-col justify-center items-center">
      <h1 class="text-4xl font-bold">{{ title }}</h1>
    </div>
  </section>
</template>

<style scoped>
.frosted-glass {
  background: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(3px);
  -webkit-backdrop-filter: blur(5px);
  padding: 20px;
}
</style>