<template>
    <div class="h-screen w-full inset-0 fixed z-50 bg-[#181a20] grid-container text-white" v-show="load">
        <div class="flex flex-col justify-center items-center gap-8 xl:gap-10 w-full h-full relative">          
            <div class="flex flex-col gap-4 xl:gap-6 items-center text-[#7636df]">
                <Icon name="mdi:fire" class="text-6xl md:text-7xl xl:text-9xl"/>
                <p class="tracking-widest text-2xl md:text-3xl xl:text-4xl text-center">FireTask</p>
            </div>
            <p class="w-full md:w-1/2 text-center md:text-lg xl:text-xl">С данным менеджером вы сможете с лёгкостью управлять своими задачами с помощью вашего устройства.</p>
            <div class="flex lg:flex-col gap-2 items-center">
                <Icon name="icon-park-outline:loading-four" class="text-lg xl:text-xl animate-spin"/>
                <p class="text-sm xl:text-base">Loading...</p>
            </div>
        </div>
    </div>
</template>

<script setup>
    const props = defineProps({
        load: Boolean
    })
</script>
