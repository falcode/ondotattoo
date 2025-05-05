<template>
  <section id="section-1">
    <div class="relative bg-transparent h-screen w-full flex flex-col justify-center items-center">
      <h1 class="text-center font-bold flex flex-col md:flex-row gap-4 mb-4 md:mb-0">
        <span>ONDO</span>
        <span>TATTOO</span>
        <span>BCN</span>
      </h1>
      <a href="https://maps.app.goo.gl/gLEj5FQRwAHTJ26y6" target="_blank">
        <p class="mt-2 text-lg">CARRER DELS MORABOS 24 BARCELONA SPAIN</p>
      </a>
    </div>

    <div ref="infoRef" class="relative z-50 flex bg-zinc-900">
      <div class="flex justify-between flex-wrap m-auto max-w-[960px] w-full p-10">

        <div class="flex flex-col p-5">
          <div class="flex flex-col mb-10 md:mb-5">
            <h2>LOCALIZACIÓN</h2>
            <p>CARRER DELS MORABOS 24</p>
            <p>BARCELONA SPAIN 08038</p>
          </div>
          <div class="flex flex-col">
            <h2 class="whitespace-pre-wrap">HORARIO</h2>
            <p>11:00 AM - 8:00 PM</p>
            <p>MARTES - SÁBADO</p>
            <p>CERRADO LUNES Y DOMINGOS</p>
          </div>
        </div>

        <div class="flex flex-col p-5">
          <h2>CONTÁCTANOS</h2>
          <p>INSTAGRAM</p>
          <p>FACEBOOK</p>
          <p>935.081.572</p>
        </div>

        <div class="flex flex-col p-5 space-y-5 max-w-sm">
          <h2>PERSONALIZADO</h2>
          <p>¿Quieres contactar con un tatuador en concreto?</p>
          <p>Cada uno tiene su propia forma de trabajar.</p>
          <p>Consulta su perfil de Instagram para más información.</p>
        </div>

      </div>

    </div>
  </section>
</template>

<script setup lang="ts">
import {ref} from "vue";

const infoRef = ref<HTMLElement | null>(null);
</script>

<style scoped>

</style>