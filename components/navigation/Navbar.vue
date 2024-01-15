<template>
    <header class="bg-cblack text-white py-4">
        <nav class="container flex justify-between mx-auto lg:px-8">
            <div>
                <NuxtLink to="/">
                    <img src="/assets/imgs/logo.svg" alt="">
                </NuxtLink>
            </div>
            <div class="flex gap-4">
                <p>+7 (888) 888 88 88</p>
                <p class="text-cred">Получить консультацию</p>
            </div>
            <div class="hidden lg:flex gap-6">
                <NuxtLink class="hover:text-cred" to="/services">Услуги</NuxtLink>
                <NuxtLink class="hover:text-cred" to="/cases">Кейсы</NuxtLink>
                <NuxtLink class="hover:text-cred" to="/faq">FAQ</NuxtLink>
            </div>
            <button class="lg:hidden"><img src="/assets/imgs/navbar/navbar-burger.svg" alt=""></button>
        </nav>
    </header>
</template>
