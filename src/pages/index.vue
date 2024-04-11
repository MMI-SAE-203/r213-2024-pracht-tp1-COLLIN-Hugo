<!-- eslint-disable vue/multi-word-component-names -->
<script setup lang="ts">
import { ref } from 'vue';

const maVar = ref(1)
console.log('maVar : ', maVar.value)
</script>

<template>
  <h1>Page d'accueil</h1>
</template>