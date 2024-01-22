<template>
    <footer class="bg-cblack">
        <div class="container mx-auto py-16">
            <div class="px-8 space-y-12">
                <div class="flex flex-col sm:flex-row justify-between items-center gap-8">
                    <div class="">
                        <img class="w-64" src="/assets/imgs/logo.svg" alt="">
                    </div>
                    <div class="flex flex-col md:flex-row justify-center items-center">
                        <div class="md:w-1/2">
                            <p class="text-cgray">Общество с ограниченной
                                ответственностью «Центр интеллектуальной собственности и инноваций „АйПиХаб“»</p>
                        </div>
                        <div class="grid grid-cols-2 md:block text-white md:w-1/5">
                            <p>123317, г. Москва, Пресненская наб., д.
                                8, стр. 1, эт. 3, п. 1, оф. 10</p>
                            <div class="flex flex-col md:flex-row gap-4">
                                <p><span class="text-cgray">ИНН:</span> 7703472433</p>
                                <p><span class="text-cgray">КПП:</span> 770301001</p>
                            </div>
                        </div>
                    </div>
                </div>
                <hr>
                <div class="flex justify-between">
                    <div class="text-white flex flex-col gap-4">
                        <h1 class="text-cgray text-[18px]">Навигация по сайту</h1>
                        <NuxtLink to="/services">Услуги</NuxtLink>
                        <NuxtLink to="/cases">Кейсы</NuxtLink>
                        <NuxtLink to="/faq">FAQ</NuxtLink>
                    </div>
                    <div class="text-white flex flex-col gap-4">
                        <h1 class="text-cgray text-[18px]">Наши контакты:</h1>
                        <a href="">example@iphub.com</a>
                        <a href="">+7 (888) 888 88 88</a>
                    </div>
                    <div class="text-white flex flex-col gap-4">
                        <h1 class="text-cgray text-[18px]">Мы в соцсетях:</h1>
                        <a href="">Facebook</a>
                        <a href="">Instagram</a>
                    </div>
                    <div class="hidden md:block text-white flex flex-col gap-4">
                        <h1 class="text-cgray text-[18px]">Как добраться:</h1>
                        <a href="">Схема проезда</a>
                    </div>
                </div>
                <div class="flex justify-between text-white">
                    <div class="text-cgray">
                        <p>© 2021 IPhub. Все права защищены.</p>
                    </div>
                    <div>
                        <p>Публичная оферта</p>
                    </div>
                    <div>
                        <p>Пользовательское соглашение</p>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>