<!-- A class that uses CSS styling equivalent to the 
 Tailwind styles in the ButtonLike component. -->
<script setup lang="ts">
interface Props {
  text: String;
}

const props = defineProps<Props>();
</script>

<template>
  <div class="buttonlike">
    <p>{{ props.text }}</p>
  </div>
</template>

<style>
.buttonlike {
  margin-left: auto;

  margin-right: auto;

  min-width: fit-content;

  border-radius: 1rem;

  border-width: 2px;

  border-color: rgb(199, 210, 254);

  background-color: rgb(238, 242, 255);

  padding: 1rem;

  text-align: center;
}
</style>
