<script setup>

defineProps(["name", "des", 'img'])

</script>

<template>
    <div class="pb-4 px-4 w-[20rem]">
        <img :src="img" alt="">
        <h1 class="text-[18px] px-2 mt-2">{{ name }}</h1>
        <p class="text-[14px] px-2">{{ des }}</p>
    </div>
</template>