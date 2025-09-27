<script setup lang="ts">
import HelloWorld from "./components/HelloWorld.vue";
import TabBar from "./components/TabBar.vue";
import ButtonBarAlts from "./examples/ButtonBarAlts.vue";
</script>

<template>
  <div class="flex p-8 min-h-48 bg-gray-100 text-center items-center">
    <h2 class="p-4 text-8xl font-semibold border-6 rounded-2xl mx-auto min-h-fit">Hello, world!</h2>
  </div>
  <TabBar :button-labels="['one', 'two', 'three', 'four']" :selected="2" />
  <HelloWorld />
</template>
