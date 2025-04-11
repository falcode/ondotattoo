<template>
  <SectionBanner title="Artistas" imgUrl="/assets/banner.png" imgAltText="Los tatuadores de Ondo Barcelona"/>
  <div class="bg-zinc-900 w-full py-2 md:p-10">
    <div class="max-w-[960px] m-auto grid grid-cols-1 md:grid-cols-4 gap-6 p-6">
      <div v-for="artist in artists" :key="artist.id"
           class="flex flex-col items-center p-4">
        <img src="/favicon.png" alt="Artist Image" class="w-[215px] h-[215px] object-contain mb-4">
        <h2 class="text-xl font-bold text-white mb-2">{{ artist.name }}</h2>
        <p class="text-gray-400 text-center mb-4">{{ artist.description }}</p>
        <a :href="artist.instagram" target="_blank" rel="noopener noreferrer"
           class="border-2 border-white text-white hover:text-zinc-900 px-4 py-2 hover:bg-white">
          Instagram
        </a>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import SectionBanner from "./SectionBanner.vue";

const artists = [
  {
    id: 1,
    name: "OSCAR HOVE",
    description: "This is a short description of Artist 1.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/oscarhove/",
  },
  {
    id: 2,
    name: "ANN WENN",
    description: "This is a short description of Artist 2.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/tattooist_ann/",
  },
  {
    id: 3,
    name: "LEONKA",
    description: "This is a short description of Artist 3.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/leonka.art/",
  },
  {
    id: 4,
    name: "BOSKN",
    description: "This is a short description of Artist 4.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/boskn_/",
  },
  {
    id: 5,
    name: "VICTOR FRANCIA",
    description: "This is a short description of Artist 5.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/victorfranciatattoo/",
  },
  {
    id: 6,
    name: "ROSTYLE",
    description: "This is a short description of Artist 6.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/rostyle_tattoo/",
  },
  {
    id: 7,
    name: "ILLMEM",
    description: "This is a short description of Artist 7.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/illmem/",
  },
  {
    id: 8,
    name: "BERTA COLOMINA",
    description: "This is a short description of Artist 8.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/menina.ttt",
  },
  {
    id: 9,
    name: "BASTIAN",
    description: "This is a short description of Artist 9.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/melgar.bastian",
  },
];
</script>

<style scoped>
</style>