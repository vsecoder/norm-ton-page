<template>
    <div class="bg-white rounded-[6px] py-[6px] px-[10px] mb-2">
        <div class="flex justify-between items-center">
            <h2 class="text-2xl" v-html="title"></h2>
            <h2 class="text-base text-[#E3E4E5]">
                {{ description }}
            </h2>
        </div>
        <img :src="image" class="mt-[6px]">
        <div class="flex flex-row gap-1 mt-[6px] text-base font-semibold">
            <a class="bg-black text-white basis-1/2 flex gap-[10px] items-center justify-center rounded-[6px] py-2" :class="color" :href="links[0]">
                <img src="/icons/tg.svg"> Telegram
            </a>
            <a class="bg-white border border-[#E3E4E5] basis-1/2 flex gap-[10px] items-center justify-center rounded-[6px] py-2" :href="links[1]">
                <img src="/icons/bh.svg"> Behance
            </a>
        </div>
    </div>
</template>

<script setup>
import { defineProps, computed } from 'vue'

const props = defineProps(['title', 'description', 'image', 'color', 'links'])

const color = computed(() => {
    return `bg-[${props.color}]`
})
</script>