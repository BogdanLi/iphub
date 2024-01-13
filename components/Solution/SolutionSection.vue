<script setup>

const solutionsArr = [
    {
        title: 'Регистрация товарного знака в Роспатенте',
        des: 'Государственная регистрация торговых знаков в РФ и в мире',
    },
    {
        title: 'Изобретения и Полезные модели',
        des: 'Изобретения и Полезные модели Регистрация прав'
    },
    {
        title: 'Промышленные образцы',
        des: 'Государственная регистрация торговых знаков в РФ и в мире'
    },
    {
        title: 'Программы для ЭВМ и Базы данных',
        des: 'Государственная регистрация торговых знаков в РФ и в мире'
    },
    {
        title: 'Представление интересов, суды',
        des: 'Государственная регистрация торговых знаков в РФ и в мире'
    },
    {
        title: 'Товарные знаки',
        des: 'Государственная регистрация торговых знаков в РФ и в мире'
    }
]

</script>

<template>
    <div class="container mx-auto lg:px-8 space-y-4 py-16">
        <div class="flex justify-between items-center">
            <div>
                <h1 class="stix text-[38px]">Решения для вашего бизнеса</h1>
                <p class="text-cgray">У нас есть все необходимые ресурсы для решения любых ваших потребностей в сфере
                    интеллектуальной собственности</p>
            </div>
            <button class="animate-arrow-btn-right border border-cred text-cred px-6 py-2 rounded-[50%] relative">Все услуги
                <img class="absolute end-[-20px] top-[40%]" src="/assets/imgs/btn-arrow.svg" alt=""></button>
        </div>
        <Swiper :slides-per-view="5" :pagination="true">
            <SwiperSlide v-for="sol in solutionsArr">
                <Solution :title="sol.title" :des="sol.des">
                </Solution>
            </SwiperSlide>
        </Swiper>
    </div>
</template>