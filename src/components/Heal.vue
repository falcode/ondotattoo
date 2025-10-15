<template>
  <section id="section-1">
    <div class="relative bg-transparent h-screen w-full flex flex-col justify-center items-center">
      <h1 class="text-center font-bold flex flex-col md:flex-row gap-4 mb-4 md:mb-0">
        <span>¿CÓMO CUIDO MI NUEVO TATUAJE?</span>
      </h1>
    </div>

    <div ref="infoRef" class="relative z-50 flex bg-zinc-900">
      <div class="flex flex-col md:flex-row max-w-7xl m-auto px-10 py-16 gap-6">
        <!-- COLUMN 1 -->
        <div class="flex flex-col gap-6">
          <div class="flex flex-col">
            <span>
              <p>Te acabas de llevar una obra de arte en la piel. Ahora toca lo más importante: que cicatrice bien para
                que luzca como merece. No es complicado, solo hay que seguir unas cuantas reglas básicas.</p>

              <h3 class="text-lg font-bold text-white mt-4 mb-2">1. No toques el tatuaje (sí, aunque tengas curiosidad)
              </h3>
              <p>Las manos sucias y los tatuajes recién hechos no son amigos. Ropa holgada, nada de estar sobando la
                zona, y deja el vendaje el tiempo que te dijo tu tatuador/a.</p>

              <h3 class="text-lg font-bold text-white mt-4 mb-2">2. Manos limpias siempre</h3>
              <p>Cada vez que lo cuides, lávate las manos. Si llevas second skin, moja con agua tibia y retírala con
                cariño, sin arrancar como si fuera una tirita de cera.</p>

              <h3 class="text-lg font-bold text-white mt-4 mb-2">3. Limpieza suave, sin dramas</h3>
              <p>Durante los 3 primeros días, lava la zona 3 veces al día con agua tibia y jabón neutro. Seca con papel
                de cocina dando toquecitos, nada de frotar ni usar la toalla del baño.</p>

              <h3 class="text-lg font-bold text-white mt-4 mb-2">4. Crema, pero sin montar una piscina encima</h3>
              <p>Aplica una capa fina con la crema hidratante para tattoos que te aconsejo tu tatuador. Lo justo para
                que la piel respire y se cure. Antes de que empiece a pelar, durante el pelado y al menos dos días más.
              </p>

              <h3 class="text-lg font-bold text-white mt-4 mb-2">5. Cada piel va a su ritmo</h3>
              <p>Algunas cicatrizan en tiempo récord, otras necesitan más calma. Lo importante: escucha a tu cuerpo. Si
                notas tirantez, hidrata un poco más. Si ves la piel saturada, dale un respiro.</p>

              <h3 class="text-lg font-bold text-white mt-4 mb-2">6. No rasques, no arranques</h3>
              <p>Aunque dé gustito. No lo hagas. Las costras y pieles tienen que caer solas. Arrancarlas = fastidiar el
                dibujo.</p>
            </span>
          </div>
        </div>

        <!-- COLUMN 2 -->
        <div class="flex flex-col gap-6">
          <div class="flex flex-col">
            <h3 class="text-lg font-bold text-white mt-4 mb-2">7. Prohibido sol, playa, piscina y sauna</h3>
            <p>Al menos dos semanas. El tatuaje tiene que estar seco y protegido. Si te da el sol, te arrepentirás (y
              nosotros también).</p>

            <h3 class="text-lg font-bold text-white mt-4 mb-2">8. Ejercicio, solo si está permitido</h3>
            <p>El sudor no es el mejor aliado en una piel que se está curando. Si tu tatuador/a no lo autorizó, espera
              a estar recuperado.</p>

            <h3 class="text-lg font-bold text-white mt-4 mb-2">9. Cuida tu piel siempre</h3>
            <p>Después de la cicatrización, sigue hidratando con tu crema favorita y protege del sol. Así el tatuaje
              se ve bonito no solo este verano, sino dentro de 10 años.</p>

            <h3 class="text-lg font-bold text-white mt-4 mb-2">10. Si algo raro pasa, avísanos</h3>
            <p>Enrojecimiento fuerte, hinchazón o secreción = escríbenos. Más vale preguntar que lamentar.</p>

            <p class="mt-4 font-semibold">La cicatrización superficial lleva entre 3 y 5 semanas. Dale tiempo y mimo,
              y el resultado será precioso.</p>

            <h3 class="text-lg font-bold text-white mt-6 mb-2">Y ahora, un último detalle:</h3>
            <p>Si te ha gustado la experiencia, deja una reseña que es gratuito. No necesitas escribir poesía: un par
              de líneas sinceras valen oro… y si además quieres añadir una foto de tu tattoo o del estudio, todavía
              mejor.</p>

            <p>Ah, y de vez en cuando hacemos sorteos para las mejores reseñas, así que tu opinión podría traerte un
              regalito.</p>

            <p>Así nos ayudas a seguir tatuando a gente maja como tú… y de paso, tus amigos sentirán envidia sana al
              ver lo bien que te ha quedado. 😉</p>

            <p class="mt-4 font-semibold">Gracias por confiar en nosotros. Tu piel y nosotros te lo agradecemos. 🖤
            </p>
          </div>

        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import { ref } from "vue";

const infoRef = ref<HTMLElement | null>(null);
</script>

<style scoped></style>