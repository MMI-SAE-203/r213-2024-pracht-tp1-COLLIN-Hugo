<script setup lang="ts">
import { ref } from 'vue';

const maVar = ref(1)
console.log('maVar : ', maVar.value)
const sectionOpen = ref(1)
</script>

<template>
  <section>
    <button class="text-xl">bouton 1</button>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates sit ad incidunt nisi commodi, exercitationem hic accusantium? Tempore magnam laborum quod error rerum, aut ipsum! Ratione velit magnam accusamus numquam?</p>
  </section>
  <section>
    <button class="text-xl">bouton 2</button>
    <p>Facilis nisi corrupti obcaecati pariatur quis? Repellendus iste, nam provident pariatur laudantium laboriosam et maiores fugiat, blanditiis, rerum velit. Quo quis reprehenderit eligendi hic sed a, aspernatur natus similique illum!</p>
  </section>
  <section>
    <button class="text-xl">bouton 3</button>
    <p>Assumenda facilis repellendus iure? Assumenda dolores modi aliquid rem esse, itaque corporis harum dolorum nisi delectus velit excepturi dicta. Quibusdam temporibus non assumenda impedit distinctio doloremque vel consectetur inventore optio?</p>
  </section>
</template>

<button @pointerdown="maVar = true?0:1">Montrer 1</button>
<h1 v-show="maVar === 1" class="text-2xl">Contenu de 1</h1>

<button @pointerdown="maVar = 2">Montrer 2</button>
<h1 v-show="maVar === 2" class="text-2xl">Contenu de 2</h1>