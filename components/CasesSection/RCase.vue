<script setup>

defineProps(['title', 'des', 'img'])

</script>

<template>
    <div class="bg-white bg-opacity-[5%] flex text-white group hover:bg-opacity-[10%]">
        <img class="absolute top-4 end-4 group-hover:opacity-0" src="/assets/imgs/solutions/arrow.svg" alt="img">
        <img class="absolute opacity-0 top-4 end-4 group-hover:opacity-100" src="/assets/imgs/solutions/hover-arrow.svg" />
        <img class="w-[12rem]" :src="img" alt="">
        <div class="flex flex-col justify-center px-4">
            <h1 class="text-[12px] md:text-[16px]">{{ title }}</h1>
            <p class="text-[10px] md:text-[14px] text-cgray">{{ des }}</p>
        </div>
    </div>
</template>