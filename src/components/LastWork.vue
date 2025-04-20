<template>
  <Banner video-url="/assets/video2.mp4" :is-full-screen=false default-img="/assets/banner.png">
    <h1 class="text-4xl font-bold">Últimos trabajos</h1>
  </Banner>

  <div ref="lastWorkRef" class="relative z-10 bg-zinc-900 w-full p-5 md:p-10 flex flex-col justify-between">
    <div class="max-w-[960px] m-auto grid grid-cols-1 md:grid-cols-3 gap-2 md:gap-6 p-3 md:p-6">
      <div v-for="work in lastwork" :key="work.id"
           class="flex flex-col items-center p-4">
        <a :href="work.url" target="_blank">
          <img :src="`/insta/${work.id}.png`" alt="Artist Image" class="w-[13em] h-[16em] object-contain">
        </a>
      </div>
    </div>
    <a href="https://www.instagram.com/ondotattoo/" target="_blank" rel="noopener noreferrer"
       class="mx-auto text-2xl mt-0 mb-5 border-2 border-white text-white hover:text-zinc-900 px-4 py-2 hover:bg-white">
      Siguenos en Instagram
    </a>
  </div>
</template>

<script setup lang="ts">
import Banner from "./Banner.vue";
import {ref} from "vue";

const lastWorkRef = ref<HTMLElement | null>(null);
const lastwork = [
  {
    id: 1,
    url: "https://www.instagram.com/p/DHmCwUcuGyU/"
  },
  {
    id: 2,
    url: "https://www.instagram.com/p/DHUB68mudlV",
  },
  {
    id: 3,
    url: "https://www.instagram.com/p/DGsbbYNIgnt/",
  },
  {
    id: 4,
    url: "https://www.instagram.com/p/DGDG0r4IHxf/",
  },
  {
    id: 5,
    url: "https://www.instagram.com/p/DC7N4unumsx/",
  },
  {
    id: 6,
    url: "https://www.instagram.com/p/DBonRSLKB45",
  },
];
</script>

<style scoped>
</style>