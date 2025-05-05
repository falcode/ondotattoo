<template>
  <section id="section-4" class="p-5 md:p-10">
    <div class="relative bg-transparent h-[40vh] w-full flex flex-col justify-center items-center">
      <h1 class="font-bold">Localización</h1>
    </div>
    <div class="relative z-50 map-container h-[450px]  w-full flex justify-center align-center">
      <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d5988.2847105113415!2d2.146508776669166!3d41.37099177130188!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x12a4a27758e88cab%3A0x88679085114a4592!2sOndo%20Tattoo%20Barcelona!5e0!3m2!1ses!2ses!4v1745251471736!5m2!1ses!2ses"
          width="600"
          height="450"
          style="border:0;"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade">>
      </iframe>
    </div>
  </section>
</template>
<script setup>
</script>
<style scoped>
.map-container iframe {
  width: 100%;
  height: 100%;
  filter: invert(1) grayscale(1);
}

</style>