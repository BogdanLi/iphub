<script setup>

const emit = defineEmits(['closeModal'])

</script>

<template>
    <div class="w-screen h-screen fixed z-50 bg-indigo top-0 left-0 bg-black/50 flex justify-center items-center"
        @click="$emit('closeModal')">
        <div class="bg-white grid grid-cols-3 w-2/3 relative rounded-lg overflow-hidden">
            <img class="cursor-pointer absolute top-4 end-4" src="@/assets/imgs/closeModal.svg" alt=""
                @click="$emit('closeModal')">
            <img class="w-full col-span-1" src="@/assets/imgs/comand/modal.png" alt="">
            <div class="col-span-2 px-4 text-cgray flex flex-col justify-center mb-4">
                <h1 class="text-[24px] text-black">Раймм Лидия Вячеславовна</h1>
                <h2>Генеральный директор</h2>
                <div class="mt-4 space-y-2">
                    <p>Создаёт тихое право сильных брендов. Строит импакт-компанию и развивает команду, которая выбрала
                        сферу
                        интеллектуальной собственности своей миссией и которая способна смело и с удовольствием превосходить
                        ожидания клиентов. Выводит в принцип работы равноценность и значимости достижения единой цели
                        с клиентом.</p>
                    <p>
                        Выбирает клиентов, как партнёров, для которых бизнес — это личное.
                    </p>
                    <p>
                        Область интересов — формирование устойчивой архитектуры систем управления интеллектуальной
                        собственностью
                        через создание честного сильного конкурентного преимущества для правообладателей.</p>
                </div>
            </div>
        </div>
    </div>
</template>