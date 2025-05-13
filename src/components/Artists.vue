<template>
  <section id="section-3">
    <div class="relative bg-transparent h-[50vh] w-full flex flex-col justify-center items-center">
      <h1 class="text-4xl font-bold">Artistas</h1>
    </div>
    <div ref="artistRef" class="relative z-50 bg-zinc-900 w-full py-2 md:p-10">
      <div class="max-w-[960px] m-auto grid grid-cols-1 md:grid-cols-3 gap-6 p-6">
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
  </section>
</template>

<script setup lang="ts">
import {ref} from "vue";

const artistRef = ref<HTMLElement | null>(null);

const artists = [
  {
    id: 1,
    name: "OSCAR HOVE",
    description: "Inspirado en el arte japonés y amante del tatuaje bien negro, Oscar tiene un estilo inconfudible, que impacta a simple vista! Hace lo difícil parecer fácil, míratelo para entender lo que te digo.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/oscarhove/",
  },
  {
    id: 2,
    name: "ANNIE",
    description: "Annie hace su propia interpretación de estilo tradicional japonés, trabaja principalmente en blanco y negro, pero también tatúa a color. La mejor manera para entenderlo, es verlo.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/tattooist_ann/",
  },
  {
    id: 3,
    name: "LEONKA",
    description: "¿Te atrae la simbología? ¿Disfrutas de las charlas intelectuales? Si esta idea te suena bien, LeonKa es tu tatuador.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/leonka.art/",
  },
  {
    id: 4,
    name: "JOSE",
    description: "Pocos controlan la línea fina como él. Si buscas este tattoo super delicado y rico en detalles, estarás en muy buenas manos.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/illmem/",
  },
  {
    id: 5,
    name: "BERTA",
    description: "Tatuajes botánicos, sus dibujos dan vida a flores silvestres, plantas, animales e insectos. Para los que buscan un tatuaje ornamental y orgánico.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/menina.ttt",
  },
  {
    id: 6,
    name: "VICTOR",
    description: "Como el mismo si define: ‘Una mezcla de técnicas y tuajes abstractos’. Este es otro que necesitas de verlo para entenderlo.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/victorfranciatattoo/",
  },
  {
    id: 7,
    name: "SEBAS",
    description: "Ilustración y black & grey, su estilo es oscuro, limpio y elegante. Tiene algo que atrapa. Míratelo… sé que tienes curiosidad.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/melgar.bastian",
  },
  {
    id: 8,
    name: "ROSS",
    description: "Hace de todo en estilo realista: desde retratos de raperos hasta el de tu perro.\nAnimales, paisajes, dioses, pelis... Además también le gusta el anime.  Ya te he dicho, lo hace todo!",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/rostyle_tattoo/",
  },
  {
    id: 9,
    name: "BOSKN",
    description: "Especializado en ilustración y blackwork, de una forma misteriosa y sombría que solo él sabe hacer.",
    image: "/public/favicon.png",
    instagram: "https://instagram.com/boskn_/",
  },
];
</script>

<style scoped>
</style>