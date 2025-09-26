<script setup lang="ts">
import ButtonBar from './components/ButtonBar.vue';
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="min-h-screen">
    <ButtonBar :button-texts="['Hello, world!', 'Hello, Stella!', 'Hello, Longnameperson!']" />
    <HelloWorld msg="Vite + Vue" />
  </div>
</template>

