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
      <div class="flex flex-col md:flex-row max-w-7xl m-auto px-10 py-16 gap-6">
        <!-- COLUMN 1 -->
        <div class="flex flex-col gap-6">
          <div class="flex flex-col">
            <h2>EL PRIMER PASO</h2>
            <span>
              <p>Puedes visitarnos en el estudio o contactarnos a través de Instagram <a
                  href="https://www.instagram.com/ondotattoo/"
                  target="_blank">@ondotattoo</a> o WhatsApp  <a href="tel:+34696708951">+34 696 708 951</a></p>
              <p>Una vez que nos contactes, por favor incluye:</p>
              <ul class="mb-4">
                <li>Una descripción clara de tu idea para el tatuaje (zona a tatuar, tamaño aproximado en cm).</li>
                <li>Referencias fotográficas o inspiración.</li>
                <li>Tu disponibilidad (fechas y horas preferidas).</li>
              </ul>
              <p>Si ya tienes elegido tu artista, por favor menciónalo en el mensaje. Si no estás seguro de quién es el más adecuado, nuestra amable manager estará feliz de ayudarte a encontrar al artista perfecto para ti.</p>
              <p>Reservamos citas hasta con 3 meses de antelación.</p>
            </span>
          </div>

          <div class="flex flex-col">
            <h2 class="whitespace-pre-wrap">¿CUÁNTO COSTARÁ MI TATTOO?</h2>
            <p>Siguiendo el primer paso, obtendrás tu presupuesto.</p>
          </div>

          <div class="flex flex-col">
            <h2>¿CÓMO DEBO PREPARARME PARA MI TATUAJE?</h2>
            <span>
            <p>Durante la semana previa a tu cita, mantén tu piel bien hidratada con la crema de tu preferencia y evita exponerte al sol.</p>
            <p>Evita salir de fiesta la noche anterior: el alcohol puede aumentar el sangrado hasta 24 horas después, lo que diluye la tinta y afecta tanto tu ánimo como el resultado del tatuaje y su cicatrización.</p>
            <p>Duerme bien y come algo antes de venir. Mantente hidratado antes y durante la sesión. Si te sientes un poco mareado, avísanos y te daremos una bebida — el azúcar es tu aliada en ese momento.</p>
            <p>Relájate y disfruta del proceso. ¡Estás en buenas manos! No hay nada de qué preocuparse.</p>
          </span>
          </div>

          <div class="flex flex-col">
            <h2>¿CÓMO CUIDO MI NUEVO TATUAJE?</h2>
            <span>
            <p>Cada estilo de tatuaje puede requerir cuidados específicos. Te entregaremos una tarjeta con instrucciones personalizadas después de tu sesión.</p>
            <p>Pero lo básico para todas las tatuajes es no exponer la zona tatuada al sol, evitar la inmersión en agua (piscina, mar, etc.) y no ir a saunas durante minimo de dos 2 semanas.</p>
          </span>
          </div>
        </div>

        <!-- COLUMN 2 -->
        <div class="flex flex-col gap-6">
          <div class="flex flex-col">
            <h2>¿DUELE?</h2>
            <span>
            <p>Sí! Tatuarse duele. Pero el dolor es muy tolerable y varía mucho de persona a persona. Depende de la zona
            del cuerpo, del tamaño y del nivel de detalle del diseño.</p>
            <p>Dicho esto, tu cerebro libera endorfinas cuando siente dolor y a tu cuerpo le encantan las endorfinas. Así
            que sí, duele… pero puede que te guste un poco y seguro que lo vás a repitir.</p>
          </span>
          </div>

          <div class="flex flex-col">
            <h2>¿CUÁNTO TIEMPO TARDA EN CURARSE UN TATUAJE?</h2>
            <span>
            <p>Tarda entre dos y tres semanas en “curarse”, pero la piel necesita varios meses para regenerarse por completo.</p>
          </span>
          </div>

          <div class="flex flex-col">
            <h2>WALK-INGS</h2>
            <span>
            <p>¿Te sientes espontáneo?</p>
            <p>Aceptamos walk-ins todos los días y se atienden por orden de llegada.</p>
            <p>La manera más rápida de consultar disponibilidad para el mismo día es llamándonos o enviando un mensaje por WhatsApp <a
                href="tel:+34696708951">+34 696 708 951</a></p>
          </span>
          </div>

          <div class="flex flex-col">
            <h2>¿OFRECEN CITAS PRIVADAS FUERA DEL ESTUDIO O EN VIAJE?</h2>
            <span>
            <p>¡Sí, lo hacemos! Escribe un email a: <a href="mailto:ondotattoo@gmail.com">ondotattoo@gmail.com</a></p>
            <p>Con el asunto: Solicitud tattoo privado</p>
          </span>
          </div>
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