<template>
    <div class="bg-white rounded-[6px] h-20 overflow-hidden relative">
        <h3 class="text-base absolute top-2 left-3">{{title}}</h3>
        <img :src="image" class="absolute right-0 bottom-0">
    </div>
</template>

<script setup>
import { defineProps } from 'vue';

const props = defineProps(['title', 'image']);
</script>