<!-- The not-recommended use of @apply and <style> together
 to make the code less hideous than using canonical Tailwind -->
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
@reference "tailwindcss";

.buttonlike {
  @apply mx-auto min-w-fit rounded-2xl border-2 border-indigo-200 bg-indigo-50 p-4 text-center;
}
</style>
