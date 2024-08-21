<template>
    <div class="grid gap-[10px] grid-cols-2 mt-1 font-semibold">
        <Stack v-for="stack in stacks" :key="stack.id" :title="stack.title" :image="stack.image" />
    </div>
</template>

<script setup>
import Stack from './Stack.vue';
import { defineProps } from 'vue';

const props = defineProps(['stacks']);
</script>