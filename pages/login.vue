<template>
    <div class="h-screen w-full inset-0 fixed z-50 bg-[#181a20] grid-container text-white">
        <div class="flex flex-col justify-center items-center gap-8 xl:gap-10 w-full h-full md:w-1/2 relative mx-auto">          
            <p class="uppercase text-xl md:text-2xl xl:text-3xl">Войдите в свой аккаунт</p>
            <form class="flex flex-col gap-4 xl:gap-6 w-full" autocomplete="off">
                <div class="w-full relative">
                    <input type="text" class="w-full px-8 py-2 rounded-lg bg-[#363942] focus:outline-none" placeholder="Логин">
                    <Icon name="material-symbols:person" class="absolute left-2 top-1/2 -translate-y-1/2 text-xl"/>
                </div>
                <div class="w-full relative">
                    <input type="password" class="w-full px-8 py-2 rounded-lg bg-[#363942] focus:outline-none" placeholder="Пароль">
                    <Icon name="material-symbols:password" class="absolute left-2 top-1/2 -translate-y-1/2 text-xl"/>
                </div>
                <button class="w-full rounded-xl py-2 bg-[#7636df] transition-colors duration-300 hover:bg-[#7636df]/70 text-center">Войти</button>
            </form>
            <div class="w-full flex items-center justify-center gap-6">
                <span class="h-px w-1/3 bg-white/50"></span>
                <p class="w-fit text-white/50">или</p>
                <span class="h-px w-1/3 bg-white/50"></span>
            </div>
            <div class="flex items-center gap-2 text-sm xl:text-base">
                <p>Нет аккаунта?</p>
                <NuxtLink to="/reg" class="text-[#7636df] transition-colors duration-300 hover:text-[#7636df]/70">Регистрация</NuxtLink>
            </div>
        </div>
    </div>
</template>

<script setup>
    useServerSeoMeta({
        title: 'Страница регистрации',
        keywords: '',
        description: '',
    })
</script>

