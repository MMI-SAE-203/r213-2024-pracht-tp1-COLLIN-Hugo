<script setup lang="ts">
    import { ref } from 'vue';
    
    const maVar = ref(1)
    console.log('maVar : ', maVar.value)
    const sectionOpen = ref(1)
    const sectionsData = [
      {
        label: 'bouton 1',
        texte: `texte panneau 1 Lorem ipsum dolor sit ame
        consectetur adipisicing elit. Inventore animi dolore,
        rerum magni laudantium quod excepturi laboriosam, 
        ex modi debitis harum reprehenderit eaque quam ut
        ea molestiae. Id, cum dolor!`
      },
      {
        label: 'bouton 2',
        texte: `texte panneau 2 Amet alias provident quos quis, 
        Officia ut ab dolores quos dolorem accusamus ad,
        consectetur unde minima, ipsum eligendi inventore id
        labore, laborum rerum laboriosam corrupti iste.
        Distinctio, perspiciatis!`
      },
      {
        label: 'bouton 3',
        texte: `texte panneau 3 Repudiandae corporis voluptates, 
        odit reprehenderit sint pariatur at voluptatum, cumque
        quia sit eligendi ex culpa eos, alias magnam molestiae
        id modi accusantium ipsa eveniet accusamus. Tempora 
        quis corporis et nam.`
      }
    ]
    const activeAccordion = ref<number | null>(null)
    </script>

<template>
    <div v-for="(section, key) in sectionsData" :key="key">
    <button class="accordion" @pointerdown="activeAccordion = activeAccordion === key ? null : key">
      {{ section.label }}
    </button>
    <div class="panel" v-show="activeAccordion === key">
      <p>{{ section.texte }}</p>
    </div>
  </div>
  </template>