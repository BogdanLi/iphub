<script setup>

defineProps(['title', 'des', 'img'])

</script>

<template>
    <div class="bg-white bg-opacity-[5%] flex text-white group hover:bg-opacity-[10%]">
        <img class="absolute top-4 end-4 group-hover:opacity-0" src="/assets/imgs/solutions/arrow.svg" alt="img">
        <img class="absolute opacity-0 top-4 end-4 group-hover:opacity-100" src="/assets/imgs/solutions/hover-arrow.svg" />
        <img :src="img" alt="">
        <div class="flex flex-col justify-center px-4">
            <h1>{{ title }}</h1>
            <p class="text-[14px] text-cgray">{{ des }}</p>
        </div>
    </div>
</template>