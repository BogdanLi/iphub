<script setup>

defineProps(['name', 'pos', 'place', 'des', 'day', 'time', 'img'])

</script>

<template>
    <div class="py-4 lg:px-4 flex flex-col sm:flex-row justify-between items-center gap-4 group">
        <div class="flex justify-start sm:flex-col md:flex-row gap-8 w-4/6 sm:w-2/6">
            <img class="aspect-square w-[8rem] h-[8rem] md:w-auto md:h-full grayscale transition-all duration-200 group-hover:grayscale-0" :src="img" alt="">
            <div class="flex flex-col justify-center">
                <h1 class="text-[14px] lg:text-1">{{ name }}</h1>
                <h1 class="text-cgray text-[12px] lg:text-[14px]">{{ pos }}</h1>
            </div>
        </div>
        <div class="w-4/6 flex">
            <div class="w-3/4 pe-4 space-y-2">
                <h1 class="text-[16px] lg:text-[18px]">{{ place }}</h1>
                <hr>
                <h1 class="text-[14px] lg:text-[16px] text-cgray">{{ des }}</h1>
            </div>
            <div class="w-1/4 flex flex-col justify-center items-center text-center">
                <h1 class="text-[18px]">{{ day }}</h1>
                <h1>{{ time }}</h1>
            </div>
        </div>
    </div>
</template>