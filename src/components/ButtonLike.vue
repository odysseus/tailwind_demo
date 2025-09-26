<script setup lang="ts">
interface Props {
    text: String;
}

const props = defineProps<Props>();
</script>

<template>
    <div class="mx-auto min-w-fit rounded-2xl border-2 border-indigo-200 bg-indigo-50 p-4 text-center">
        <p>{{ props.text }}</p>
    </div>
</template>