<script setup>

defineProps(['title', 'des', 'link'])

</script>

<template>
    <div class="solution group">
        <img class="absolute top-4 end-4 group-hover:opacity-0" src="/assets/imgs/solutions/arrow.svg" alt="img">
        <img class="absolute opacity-0 top-4 end-4 group-hover:opacity-100" src="/assets/imgs/solutions/hover-arrow.svg"
            alt="">
        <div>
            <img class="group-hover:scale-[.9]" :src="link" alt="image">
        </div>
        <h1 class="group-hover:translate-y-0 group-hover:text-white">{{ title }}</h1>
        <p class="group-hover:opacity-100 group-hover:translate-y-0">{{ des }}</p>
    </div>
</template>