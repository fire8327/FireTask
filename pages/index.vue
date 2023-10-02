<template>
    <div class="flex flex-col items-center justify-center gap-10 md:gap-12 xl:gap-16 h-screen text-center">
        <Swiper :slides-per-view="1" :loop="true" :autoplay="false" class="w-full">
            <SwiperSlide class="!flex flex-col gap-16 md:gap-20 xl:gap-24 w-full items-center">
                <img src="/images/startSlider/time.png" alt="" class="w-24 md:w-28 xl:w-32">          
                <div class="flex flex-col gap-4 items-center w-full md:w-1/2">
                    <p class="uppercase text-xl md:text-2xl xl:text-3xl">Наслаждайтесь своим временем</p>
                    <p class="md:text-lg xl:text-xl text-[#363942]">Если вы не уверены в том, как справиться со своей задачей, приходите к нам</p>
                </div>           
            </SwiperSlide>
            <SwiperSlide class="!flex flex-col gap-16 md:gap-20 xl:gap-24 w-full items-center">
                <img src="/images/startSlider/calendar.png" alt="" class="w-24 md:w-28 xl:w-32">       
                <div class="flex flex-col gap-4 items-center w-full md:w-1/2">
                    <p class="uppercase text-xl md:text-2xl xl:text-3xl">Организуйте свои задачи легко</p>
                    <p class="md:text-lg xl:text-xl text-[#363942]">С нами вы можете создавать, редактировать и удалять свои задачи</p>
                </div>             
            </SwiperSlide>
            <SwiperSlide class="!flex flex-col gap-16 md:gap-20 xl:gap-24 w-full items-center">
                <img src="/images/startSlider/app.png" alt="" class="w-24 md:w-28 xl:w-32"> 
                <div class="flex flex-col gap-4 items-center w-full md:w-1/2">
                    <p class="uppercase text-xl md:text-2xl xl:text-3xl">Всё в одном приложеннии</p>
                    <p class="md:text-lg xl:text-xl text-[#363942]">Всё, что вам нужно и в одном месте абсолютно бесплатно</p>
                </div>
            </SwiperSlide>
        </Swiper>
        <div class="flex max-xl:flex-col gap-4 items-center justify-center w-full md:w-1/2">
            <NuxtLink to="/" class="w-full xl:w-1/2 rounded-xl py-2 bg-[#7636df]">Вход</NuxtLink>
            <NuxtLink to="/" class="w-full xl:w-1/2 rounded-xl py-2 bg-[#363942]">Регистрация</NuxtLink>
        </div>
    </div>
</template>

<script setup>
    useServerSeoMeta({
        title: 'Стартовая страница',
        keywords: '',
        description: '',
    })
</script>
