<script setup lang="ts">
import { ref } from 'vue';

const maVar = ref(1)
console.log('maVar : ', maVar.value)
</script>

<template>
  <button @pointerdown="maVar = true?0:1">Montrer 1</button>
  <h1 v-show="maVar === 1 class="text-2xl">Contenu de 1</h1>

  <button @pointerdown="maVar = 2">Montrer 2</button>
  <h1 v-show="maVar === 2" class="text-2xl">Contenu de 2</h1>
</template>