<script setup>
const props = defineProps(['img'])
const companies = {
    depot: '/assets/imgs/partners/depot.svg',
    metafax: '/assets/imgs/partners/metafax.svg',
    deneb: '/assets/imgs/partners/deneb.svg',
    mone: '/assets/imgs/partners/mone.svg',
    betcity: '/assets/imgs/partners/betcity.svg',
    fisho2: '/assets/imgs/partners/fisho2.svg'
}
// console.log(props);
</script>

<template>
    <div class="bg-white bg-opacity-[5%] flex justify-center items-center p-4">
        <!-- <h1>{{ img }}</h1> -->
        <img :src="companies[img]" alt="">
    </div>
</template>