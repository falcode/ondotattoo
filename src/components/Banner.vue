<template>
  <section class="w-full h-screen bg-cover bg-center flex flex-col justify-center items-center text-center text-white"
           style="background-image: url('/src/assets/banner.png');">
    <div class="frosted-glass w-full h-full flex flex-col justify-center items-center">
      <h1 class="text-4xl font-bold">ONDO TATTOO BCN</h1>
      <a href="https://maps.app.goo.gl/gLEj5FQRwAHTJ26y6" target="_blank">
        <p class="mt-2 text-lg"> CARRER DELS MORABOS 24 BARCELONA SPAIN</p>
      </a>
    </div>
  </section>
</template>

<style scoped>
.frosted-glass {
  background: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(3px);
  -webkit-backdrop-filter: blur(5px);
  padding: 20px
}
</style>
<script setup lang="ts">
</script>