<script setup lang="ts">
import ButtonLike from './ButtonLike.vue';

interface Props {
    buttonTexts: string[];
}

const props = defineProps<Props>();
</script>

<template>
    <div class="flex bg-amber-50 p-4">
        <ButtonLike v-for="label in props.buttonTexts" :text="label" />
    </div>
</template>