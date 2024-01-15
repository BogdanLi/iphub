<script setup>

const cards = [
    { title: 'CIRKLE — производитель косметической продукции', des: 'Как в результате защиты  мы зарегистрировали бренд российской косметики при наличии оснований для отказа', link: '' },
    { title: 'Camera IQ — производитель систем машинного зрения', des: 'Защита прав после ребрендинга. Как провести успешную регистрацию', link: '' },
    { title: 'HANDS — производитель строительных материалов', des: 'Предварительный отказ — не приговор! Как мы защищали монополию российского производителя строительных материалов.', link: '' }
]

</script>

<template>
    <div class="bg-cblack py-16">
        <div class="container mx-auto px-8 space-y-6">
            <div class="flex justify-between items-center">
                <div class="text-white w-1/2">
                    <h1 class="text-[38px] stix">Реализованные кейсы</h1>
                    <p class="text-cgray">Наши реальные истории о том, как мы помогали своим клиентам регистрировать
                        товарные знаки и оформлять
                        права на объекты интеллектуальной собственности</p>
                </div>
                <button class="animate-arrow-btn-right border border-cred text-cred px-6 py-2 rounded-[50%] relative">Далее
                    <img class="absolute end-[-20px] top-[40%]" src="/assets/imgs/btn-arrow.svg" alt=""></button>
            </div>
            <Swiper :slides-per-view="2" :pagination="true">
                <SwiperSlide class="me-4" v-for="card in cards">
                    <RCase :title="card.title" :des="card.des">
                    </RCase>
                </SwiperSlide>
            </Swiper>
        </div>
    </div>
</template>