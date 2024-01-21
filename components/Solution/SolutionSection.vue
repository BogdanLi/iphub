<script setup>

import img1 from '@/assets/imgs/solutions/registration.svg';
import img2 from '@/assets/imgs/solutions/inven.svg'
import img3 from '@/assets/imgs/solutions/examp.svg'
import img4 from '@/assets/imgs/solutions/db.svg'
import img5 from '@/assets/imgs/solutions/court.svg'
import img6 from '@/assets/imgs/solutions/license.svg'

const solutionsArr = [
    {
        title: 'Регистрация товарного знака в Роспатенте',
        des: 'Государственная регистрация торговых знаков в РФ и в мире',
        link: img1
    },
    {
        title: 'Изобретения и Полезные модели',
        des: 'Изобретения и Полезные модели Регистрация прав',
        link: img2
    },
    {
        title: 'Промышленные образцы',
        des: 'Государственная регистрация торговых знаков в РФ и в мире',
        link: img3
    },
    {
        title: 'Программы для ЭВМ и Базы данных',
        des: 'Государственная регистрация торговых знаков в РФ и в мире',
        link: img4
    },
    {
        title: 'Представление интересов, суды',
        des: 'Государственная регистрация торговых знаков в РФ и в мире',
        link: img5
    },
    {
        title: 'Товарные знаки',
        des: 'Государственная регистрация торговых знаков в РФ и в мире',
        link: img6
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
        <Swiper class="md:!hidden" :modules="[SwiperNavigation]" :slides-per-view="2" :navigation="true">
            <SwiperSlide v-for="sol in solutionsArr">
                <Solution :title="sol.title" :des="sol.des" :link="sol.link">
                </Solution>
            </SwiperSlide>
        </Swiper>
        <Swiper class="!hidden md:!block lg:!hidden" :modules="[SwiperNavigation]" :slides-per-view="2" :navigation="true">
            <SwiperSlide v-for="sol in solutionsArr">
                <Solution :title="sol.title" :des="sol.des" :link="sol.link">
                </Solution>
            </SwiperSlide>
        </Swiper>
        <Swiper class="!hidden lg:!block" :modules="[SwiperNavigation]" :slides-per-view="4" :navigation="true">
            <SwiperSlide v-for="sol in solutionsArr">
                <Solution :title="sol.title" :des="sol.des" :link="sol.link">
                </Solution>
            </SwiperSlide>
        </Swiper>
    </div>
</template>