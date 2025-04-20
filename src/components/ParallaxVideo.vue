<!-- src/components/ParallaxVideo.vue -->
<template>
  <template v-for="video in videos">
    <div :id="`video-${video.id}`" class="parallax-video-container">
      <video
          :id="`player-${video.id}`"
          :src="video.src"
          :autoplay="true"
          :loop="true"
          :muted="true"
          playsinline
          class="parallax-video"
      ></video>
    </div>
  </template>
</template>

<script setup>
import {onMounted, onUnmounted} from 'vue'

const handleScroll = () => {

  requestAnimationFrame(() => {
    videos.forEach((video) => {
      const sectionElement = document.getElementById(`section-${video.id}`);
      const videoElement = document.getElementById(`video-${video.id}`);
      const playerElement = document.getElementById(`player-${video.id}`);

      if (sectionElement && videoElement && playerElement) {
        const rect = sectionElement.getBoundingClientRect();
        const distanceFromTop = window.scrollY - sectionElement.offsetTop;

        if (rect.bottom < 0 || rect.top > window.innerHeight) {
          videoElement.style.transform = `translate3d(0, -100%, 0)`;
        } else {
          videoElement.style.transform = `translate3d(0, ${-distanceFromTop}px, 0)`;
        }

        playerElement.style.transform = `translateY(${distanceFromTop * 0.8}px)`;
      }
    });
  });
};

onMounted(() => {
  window.addEventListener('scroll', handleScroll, {passive: true});
});

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
});

const videos = [
  {
    src: '/assets/video.mp4',
    id: '1'
  },
  {
    src: '/assets/video2.mp4',
    id: '2'
  },
  {
    src: '/assets/video.mp4',
    id: '3'
  }
]
</script>

<style scoped>
.parallax-video-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  overflow-x: hidden;
  overflow-y: hidden;
  backface-visibility: hidden;
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