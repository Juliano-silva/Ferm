<template>
  <div id="Corpo4">
  <h1>Escreva o Link do site</h1>
  <input v-model="InputText" placeholder="Link do site" for="name" filled/>
  <iframe :src=InputText frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
</template>
<script setup>
import {ref} from 'vue'
const InputText = ref('https://www.youtube.com/embed/WVBasDB8A8c')
</script>
