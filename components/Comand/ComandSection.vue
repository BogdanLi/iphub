<script setup>

import lidiya from '@/assets/imgs/comand/lidiya.png'
import gena from '@/assets/imgs/comand/gena.png'
import ekaterina from '@/assets/imgs/comand/ekaterina.png'
import yulia from '@/assets/imgs/comand/yulia.png'
import alina from '@/assets/imgs/comand/alina.png'

const cards = [
    { name: 'Раймм Лидия Вячеславовна', des: 'Генеральный директор', link: lidiya },
    { name: 'Золотов Геннадий Борисович', des: 'Руководитель отдела патентно-юридического делопроизводства', link: gena },
    { name: 'Осоргина Екатерина Александровна', des: 'Патентный поверенный РФ', link: ekaterina },
    { name: 'Рачеева Юлия Геннадьевна', des: 'Патентный поверенный РФ', link: yulia },
    { name: 'Пахоменко Алина Аликовна', des: 'Адвокат', link: alina }
]

</script>

<template>
    <div class="py-16">
        <div class="container lg:mx-auto lg:px-8">
            <div class="w-1/2">
                <h1 class="text-[38px] stix">Команда экспертов</h1>
                <p class="text-cgray">Наша команда — эксперты в сфере IP. Мы берёмся за работу и доводим дело до конца,
                    потому что понимаем
                    ценности вашего бизнеса</p>
            </div>
        </div>
        <div>
            <Swiper :slides-per-view="5">
                <SwiperSlide v-for="card in cards">
                    <ComandCard :name="card.name" :des="card.des" :img="card.link" />
                </SwiperSlide>
            </Swiper>
        </div>
    </div>
</template>