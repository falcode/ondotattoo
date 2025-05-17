<template>
  <section id="section-2">
    <div class="relative bg-transparent h-[50vh] w-full flex flex-col justify-center items-center">
    </div>

    <div ref="lastWorkRef" class="relative z-50 bg-zinc-900 w-full p-5 md:p-10 flex flex-col justify-between">
      <div class="max-w-[960px] m-auto grid grid-cols-1 md:grid-cols-3 gap-4">
        <div v-for="work in lastwork" :key="work.id"
             class="flex flex-col items-center p-4">
          <a :href="work.url" target="_blank">
            <div class="w-full aspect-w-1 aspect-h-1">
              <img :src="`/insta/${work.id}.png`" alt="Artist Image" class="w-full h-full object-cover object-center">
            </div>
          </a>
        </div>
      </div>
      <a href="https://www.instagram.com/ondotattoo/" target="_blank" rel="noopener noreferrer"
         class="mx-auto text-2xl mt-0 mb-5 border-2 border-white text-white hover:text-zinc-900 px-4 py-2 hover:bg-white">
        Siguenos en Instagram
      </a>
    </div>
  </section>
</template>

<script setup lang="ts">
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
    url: "https://www.instagram.com/p/DD-E2LDOuAD",
  },
  {
    id: 7,
    url: "https://www.instagram.com/p/DEp-rc9OOeJ",
  },
  {
    id: 8,
    url: "https://www.instagram.com/p/DDuwHzEuIBj",
  },
  {
    id: 9,
    url: "https://www.instagram.com/p/DBq0Picqwq7",
  },
];
</script>

<style scoped>
</style>