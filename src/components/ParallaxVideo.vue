<template>
  <template v-for="video in props.videos">
    <div :id="`video-${video.id}`"
      :class="`parallax-video-container ${video.isFullscreen ? 'parallax-video-container-fullscreen' : ''}`">
      <video :id="`player-${video.id}`" :src="video.src" :autoplay="true" :loop="true" :muted="true" playsinline
        class="parallax-video"></video>
    </div>
  </template>
</template>

<script setup lang="ts">
import { onMounted, onUnmounted } from 'vue'

interface Video {
  src: string;
  id: string;
  isFullscreen: boolean;
}

const props = defineProps < {
  videos: Video[]
} > ();

const handleScroll = () => {

  requestAnimationFrame(() => {
    props.videos.forEach((video) => {
      const sectionElement = document.getElementById(`section-${video.id}`);
      const videoElement = document.getElementById(`video-${video.id}`);
      const playerElement = document.getElementById(`player-${video.id}`);

      if (sectionElement && videoElement && playerElement) {
        const rect = sectionElement.getBoundingClientRect();
        const distanceFromTop = window.scrollY - sectionElement.offsetTop;

        if (rect.bottom < 0 || rect.top > window.innerHeight) {
          videoElement.style.transform = `translate3d(0, -100%, 0)`;
        } else {
          let translateY = Math.round(-distanceFromTop);
          translateY += video.id === '1' ? 0 : -100;
          videoElement.style.transform = `translate3d(0, ${translateY}px, 0)`;
        }
        const playerTranslateY = Math.round(distanceFromTop * 0.8);
        playerElement.style.transform = `translateY(${playerTranslateY * 0.8}px)`;
      }
    });
  });
};

onMounted(() => {
  window.addEventListener('scroll', handleScroll, { passive: true });
});

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
});
</script>

<style scoped>
.parallax-video-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  overflow: hidden;
  backface-visibility: hidden;
}

.parallax-video-container-fullscreen {
  height: 110vh;
}

.parallax-video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 0;
  overflow: hidden;
  pointer-events: none;
  display: block;
  object-fit: cover;
}
</style>