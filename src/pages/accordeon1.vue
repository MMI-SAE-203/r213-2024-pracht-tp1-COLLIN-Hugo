<!-- eslint-disable vue/multi-word-component-names -->
<script setup lang="ts">
import { ref } from 'vue';

const maVar = ref(1)
console.log('maVar : ', maVar.value)
const sectionOpen = ref(1)
</script>

<template>
    <section>
      <button class="text-xl" @pointerdown="sectionOpen = sectionOpen === 1?0:1">bouton 1</button>
      <p v-show="sectionOpen === 1">Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates sit ad incidunt nisi commodi, exercitationem hic accusantium? Tempore magnam laborum quod error rerum, aut ipsum! Ratione velit magnam accusamus numquam?</p>
    </section>
    <section>
      <button class="text-xl" @pointerdown="sectionOpen = sectionOpen === 2?0:2">bouton 2</button>
      <p v-show="sectionOpen === 2">Facilis nisi corrupti obcaecati pariatur quis? Repellendus iste, nam provident pariatur laudantium laboriosam et maiores fugiat, blanditiis, rerum velit. Quo quis reprehenderit eligendi hic sed a, aspernatur natus similique illum!</p>
    </section>
    <section>
      <button class="text-xl" @pointerdown="sectionOpen = sectionOpen === 3?0:3">bouton 3</button>
      <p v-show="sectionOpen === 3">Assumenda facilis repellendus iure? Assumenda dolores modi aliquid rem esse, itaque corporis harum dolorum nisi delectus velit excepturi dicta. Quibusdam temporibus non assumenda impedit distinctio doloremque vel consectetur inventore optio?</p>
    </section>
</template>