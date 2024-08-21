<template>
    <div class="mt-2">
        <Card v-for="card in cards" :key="card.id" :title="card.title" :description="card.description" :image="card.image" :color="card.color" :links="card.links" />
    </div>
</template>

<script setup>
import Card from './Card.vue';
import { defineProps } from 'vue';

const props = defineProps(['cards']);
</script>