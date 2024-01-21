<script setup>

defineProps(['name', 'pos', 'place', 'des', 'day', 'time', 'img'])

</script>

<template>
    <div class="py-4 lg:px-4 flex justify-between items-center gap-4 group">
        <div class="flex gap-8 lg:w-2/6">
            <img class="!aspect-square grayscale transition-all duration-200 group-hover:grayscale-0" :src="img" alt="">
            <div class="flex flex-col justify-center">
                <h1>{{ name }}</h1>
                <h1 class="text-cgray text-[14px]">{{ pos }}</h1>
            </div>
        </div>
        <div class="lg:w-3/6 pe-4 space-y-2">
            <h1 class="text-[18px]">{{ place }}</h1>
            <hr>
            <h1 class="text-cgray">{{ des }}</h1>
        </div>
        <div class="lg:w-1/6 flex flex-col items-center">
            <h1 class="text-[18px]">{{ day }}</h1>
            <h1>{{ time }}</h1>
        </div>
    </div>
</template>