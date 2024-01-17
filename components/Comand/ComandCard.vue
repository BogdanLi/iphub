<script setup>

defineProps(["name", "des", 'img'])

const emit = defineEmits(['closeModal'])

</script>

<template>
    <div class="pb-4 px-4 w-[20rem] group cursor-pointer" @click="$emit('closeModal')">
        <div class="overflow-hidden">
            <img class="grayscale transition-all overflow-hidden group-hover:grayscale-0 group-hover:scale-110" :src="img"
                alt="">
        </div>
        <h1 class="text-[18px] px-2 mt-2">{{ name }}</h1>
        <p class="text-[14px] px-2">{{ des }}</p>
    </div>
</template>