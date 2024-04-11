<script setup lang="ts">
import { ref } from 'vue';

const maVar = ref(1)
console.log('maVar : ', maVar.value)
const sectionOpen = ref(1)
</script>

<template>
  <h1>Page d'accueil</h1>
</template>