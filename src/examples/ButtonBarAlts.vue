<script setup lang="ts">
import ButtonBar from "../components/ButtonBar.vue";
import ButtonClassic from "../components/ButtonClassic.vue";
import AppliedButton from "../components/AppliedButton.vue";
</script>

<template>
  <div>
    <ButtonBar
      :button-texts="[
        'Hello, world!',
        'Hello, Stella!',
        'Hello, Longnameperson!',
      ]"
    />
    <div class="flex bg-fuchsia-100 p-4">
      <ButtonClassic text="Hello, world!" />
      <ButtonClassic text="Hello, Stella!" />
      <ButtonClassic text="Hello, Longnameperson!" />
    </div>
    <div class="flex bg-lime-100 p-4">
      <AppliedButton text="Hello, world!" />
      <AppliedButton text="Hello, Stella!" />
      <AppliedButton text="Hello, Longnameperson!" />
    </div>
  </div>
</template>
