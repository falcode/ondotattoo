<template>
  <section class="relative w-full h-screen flex flex-col justify-center items-center text-center text-white">
    <!-- SEO-friendly image -->
    <img src="/assets/banner.png" alt="Banner description" class="absolute inset-0 w-full h-full object-cover"/>

    <!-- Content overlay -->
    <div class="frosted-glass relative z-10 w-full h-full flex flex-col justify-center items-center">
      <h1 class="text-4xl font-bold">ONDO TATTOO BCN</h1>
      <a href="https://maps.app.goo.gl/gLEj5FQRwAHTJ26y6" target="_blank">
        <p class="mt-2 text-lg">CARRER DELS MORABOS 24 BARCELONA SPAIN</p>
      </a>
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