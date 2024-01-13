<template>
    <div class="bg-cred py-16">
        <div class="container mx-auto px-8 space-y-6">
            <div class="text-white">
                <h1 class="stix text-[38px]">Не знаете, что вам нужно?</h1>
                <p>Пройдите квиз, чтобы выбрать оптимальное решение для Вашей задачи</p>
            </div>
            <div>
                <Quiz />
            </div>
            <div class="space-y-4">
                <h1 class="text-white text-[24px]">Бонусы после прохождения</h1>
                <div class="flex gap-8">
                    <div class="bg-cblack flex justify-center items-center p-4 w-[26rem] rounded-lg">
                        <img src="/assets/imgs/bonus.svg" alt="">
                        <p class="text-[18px] text-white">Название бонуса в одну или две строки</p>
                    </div>
                    <div class="bg-cblack flex justify-center items-center p-4 w-[26rem] rounded-lg">
                        <img src="/assets/imgs/bonus.svg" alt="">
                        <p class="text-[18px] text-white">Название бонуса в одну или две строки</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>