<template>
    <div class="bg-[#F8F8F8] w-full">
        <div class="p-8 font-semibold mx-auto max-w-sm">
            <div class=" flex justify-between">
                <div>
                    <h3 class="text-base">
                        It's norm <img src="/favicon.svg" class="inline-block mx-1"> <span
                            class="text-[#007AFF]">.ton</span>
                        page
                    </h3>
                    <h1 class="text-5xl">
                        <span class="text-[#007AFF]">Hi</span> everyone
                        </h1>
                    </div>
                    <a class="w-[30px] max-h-[30px] bg-white rounded-[10px] flex items-center justify-center" href="https://tonviewer.com/uxdesigner.ton">
                        <img src="/wallet.svg">
                    </a>
            </div>

            <div class="mt-5">
                <h2 class="text-2xl">
                    <span class="text-[#007AFF]">My</span> Stack
                </h2>

                <Stacks :stacks="stacks" />
            </div>

            <div class="mt-10">
                <h2 class="text-2xl">
                    Portfolio
                </h2>

                <Cards :cards="cards" />
            </div>
        </div>
    </div>
</template>

<script setup>
import Stacks from './components/Stacks.vue';
import Cards from './components/Cards.vue';

const stacks = [
    {
        id: 1,
        title: "Web Design",
        image: "/stack/1.png"
    },
    {
        id: 2,
        title: "Brand Design",
        image: "/stack/2.png"
    },
    {
        id: 3,
        title: "Graphic Design",
        image: "/stack/3.png"
    },
    {
        id: 4,
        title: "And other",
        image: "/stack/4.png"
    }
]

const cards = [
    {
        id: 1,
        title: "<span class='text-[#007AFF]'>BFG</span> Project",
        description: "Brand design",
        image: "/portfolio/bfg.png",
        color: "#007AFF",
        links: ['https://t.me/noneportfolio/331', 'https://www.behance.net/gallery/201917119/ITD-FEST-IDENTITY']
    },
    {
        id: 2,
        title: "<span class='text-[#5477D6]'>GO</span>",
        description: "Brand design",
        image: "/portfolio/go.png",
        color: "#5477D6",
        links: ['https://t.me/noneportfolio/347', 'https://www.behance.net/gallery/203699261/GO-prokat-samokatov']
    },
    {
        id: 3,
        title: "It’s <span class='text-[#B9EA44]'>Design</span>",
        description: "Brand design",
        image: "/portfolio/itd.png",
        color: "#1D1D1B",
        links: ['https://t.me/noneportfolio/358', 'https://www.behance.net/gallery/205747815/BFG-Game-Bot-Telegram-Bot-Mini-App']
    }
]
</script>

