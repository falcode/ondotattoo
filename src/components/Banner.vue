<script setup lang="ts">
import {defineProps} from 'vue';

const props = defineProps({
  videoUrl: {
    type: String,
    required: true,
  },
  isFullScreen: {
    type: Boolean,
    default: false,
  },
  defaultImg: {
    type: String,
    default: '/assets/banner.png',
  },
});
</script>

<template>
  <section
      :class="`relative w-full overflow-hidden ${isFullScreen ? 'h-screen' : 'h-[50vh]'} flex flex-col justify-center items-center text-center text-white`"
  >
    <!-- Background video with fallback image -->
    <div class="absolute top-0 left-0 w-full h-full z-0">
      <video
          class="w-full h-full object-cover"
          autoplay
          muted
          loop
          playsinline
      >
        <source :src="videoUrl" type="video/mp4"/>
        <img :src="defaultImg" alt="Fallback image" class="w-full h-full object-cover"/>
      </video>
    </div>

    <!-- Foreground content -->
    <div class="relative z-10 w-full h-full flex flex-col justify-center items-center">
      <slot/>
    </div>
  </section>
</template>

<style scoped>
/* Optional: fade effect or parallax illusion can be added here */
</style>
