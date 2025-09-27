<script setup lang="ts">
import HelloWorld from "./components/HelloWorld.vue";
import TabBar from "./components/TabBar.vue";
</script>

<template>
  <div class="flex min-h-48 bg-gray-100 p-8">
    <h2 class="mx-auto my-auto rounded-2xl border-6 p-4 text-8xl font-semibold">
      Hello, world!
    </h2>
  </div>
  <TabBar :button-labels="['one', 'two', 'three', 'four']" :selected="2" />
  <HelloWorld />
</template>
