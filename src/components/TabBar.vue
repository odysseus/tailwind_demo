<script setup lang="ts">
interface Props {
  buttonLabels: string[];
  selected: number;
}

const props = defineProps<Props>();
</script>

<template>
  <div class="bar">
    <div class="relative" v-for="(label, index) in buttonLabels">
      <div
        :class="{
          tab: true,
          behind: index != props.selected,
          selected: index == props.selected,
        }"
      >
        <p>{{ label }}</p>
      </div>
      <div :class="{ hideShadow: index == props.selected }"></div>
    </div>
  </div>
</template>

<style>
@reference "tailwindcss";

.bar {
  @apply flex bg-gray-100 pt-4 pl-4;
}

.tab {
  @apply ml-2 max-w-fit min-w-32 rounded-t-3xl border-gray-200 bg-white p-4 text-center;
}

.behind {
  @apply border-b-2;
}

.selected {
  @apply border-x-2 border-t-2 font-semibold shadow-[0_0_5px_gray];
}

.hideShadow {
  @apply absolute -bottom-2 h-2 w-36 bg-amber-100;
}
</style>
