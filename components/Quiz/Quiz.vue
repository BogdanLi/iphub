<script setup>

const quizItems = ['Регистрацию полезной модели', 'Регистрацию прав на использование полезной модели, промобразца, изобретенния', 'Регистрацию изобретения', 'Регистрацию промышленного образца', 'Подготовка заявки на выдачу патента', 'Подготовка заявки на передачу прав патента']

const page = ref(2)

</script>

<template>
    <div class="bg-cblack rounded-lg p-8 space-y-4 lg:w-2/3">
        <div class="flex justify-between">
            <h1 class="text-white text-[24px]">С какой целью вы обращаетесь?</h1>
            <p class="text-white stix text-[36px]"><span class="text-cred">{{ page }}</span>/8</p>
        </div>
        <div class="grid grid-cols-2 gap-4">
            <div v-for="item in quizItems">
                <QuizItem :text="item" />
            </div>
        </div>
        <div class="flex justify-between">
            <button @click="page === 0 ? page : page--"
                class="animate-arrow-btn-left border border-cred text-cred px-6 py-2 rounded-[50%] relative">Назад
                <img class="absolute start-[-20px] top-[40%]" src="/assets/imgs/btn-arrow-left.svg" alt=""></button>
            <button @click="page === 8 ? page : page++"
                class="animate-arrow-btn-right border border-cred text-cred px-6 py-2 rounded-[50%] relative">Далее
                <img class="absolute end-[-20px] top-[40%]" src="/assets/imgs/btn-arrow.svg" alt=""></button>
        </div>
    </div>
</template>