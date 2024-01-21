<script setup>

import lid from '@/assets/imgs/forums/lid.png'
import gen from '@/assets/imgs/forums/gen.png'

const future = ref(true)

const futureForums = [
    { author: 'Раймм Лидия Вячеславовна', position: 'Генеральный директор IPhub', place: 'Менторская гостинная', des: 'Индивидуальная 30-ти минутная сессия с разбором вашего кейса.', day: '9-10 ноября', time: '18:00', img: lid },
    { author: 'Золотов Геннадий Борисович', position: 'Руководитель отдела патентно-юридического делопроизводства', place: 'WIPO SUMMER SCHOOL — 2021 RUSSIA', des: 'Летняя школа Всемирной организации интеллектуальной собственности', day: '28 июня - 9 июля', time: '15:30', img: gen }
]
const pastForumes = [
    { author: 'Осоргина Екатерина Александровна', position: 'Патентный поверенный РФ', place: 'Менторская гостинная', des: 'Индивидуальная 30-ти минутная сессия с разбором вашего кейса.', day: '9-10 ноября', time: '18:00', img: lid },
    { author: 'Рачеева Юлия Геннадьевна', position: 'Патентный поверенный РФ', place: 'WIPO SUMMER SCHOOL — 2021 RUSSIA', des: 'Летняя школа Всемирной организации интеллектуальной собственности', day: '28 июня - 9 июля', time: '15:30', img: gen }
]

</script>

<template>
    <div class="py-16">
        <div class="container lg:mx-auto lg:px-8">
            <div class="flex justify-between">
                <h1 class="text-[24px]">Мы на форумах</h1>
                <div class="text-gray space-x-4">
                    <button @click="future = false" :class="!future ? 'text-cred' : 'text-gray'">Прошедшие</button>
                    <button @click="future = true" :class="future ? 'text-cred' : 'text-gray'">Будущие</button>
                </div>
            </div>
            <div>
                <div v-for="f in (future ? futureForums : pastForumes)">
                    <Event :name="f.author" :pos="f.position" :place="f.place" :des="f.des" :day="f.day" :time="f.time"
                        :img="f.img" />
                </div>
            </div>
        </div>
    </div>
</template>