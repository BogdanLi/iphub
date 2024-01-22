<script setup>

const showSidebar = ref(false)

</script>

<template>
    <header class="bg-cblack text-white py-4">
        <nav class="container flex justify-between mx-auto lg:px-8">
            <div>
                <NuxtLink to="/">
                    <img src="/assets/imgs/logo.svg" alt="">
                </NuxtLink>
            </div>
            <div class="hidden md:block flex gap-4">
                <p>+7 (888) 888 88 88</p>
                <p class="text-cred">Получить консультацию</p>
            </div>
            <div class="hidden lg:flex gap-6">
                <NuxtLink class="hover:text-cred" to="/services">Услуги</NuxtLink>
                <NuxtLink class="hover:text-cred" to="/cases">Кейсы</NuxtLink>
                <NuxtLink class="hover:text-cred" to="/faq">FAQ</NuxtLink>
            </div>
            <button @click="showSidebar = true" class="lg:hidden"><img src="/assets/imgs/navbar/navbar-burger.svg"
                    alt=""></button>
        </nav>
    </header>
    <div :class="showSidebar ? 'z-50 opacity-100' : 'z-[-1] opacity-0'" @click="showSidebar = false"
        class="w-screen h-screen fixed z-50 bg-indigo top-0 left-0 bg-black/50 flex justify-start items-center transition-all">
        <div class="w-1/2 flex transition-all duration-300" :class="showSidebar ? 'translate-x-0' : 'translate-x-[-100%]'">
            <div class="h-screen bg-cgray w-1/3"></div>
            <div class="h-screen bg-cblack w-2/3 text-white text-xl sm:text-3xl flex flex-col justify-start pt-12 ps-12 sm:pt-24 sm:ps-24 gap-8">
                <NuxtLink class="hover:text-cred" to="/services">Услуги</NuxtLink>
                <NuxtLink class="hover:text-cred" to="/cases">Кейсы</NuxtLink>
                <NuxtLink class="hover:text-cred" to="/faq">FAQ</NuxtLink>
            </div>
        </div>
    </div>
</template>
