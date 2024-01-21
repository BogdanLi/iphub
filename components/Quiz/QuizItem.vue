<script setup>

defineProps(['text'])

const active = ref(false)

</script>

<template>
    <div @click="active = !active" class="text-[14px] p-2 lg:p-8 text-white h-20 flex items-center cursor-pointer"
        :class="active ? 'bg-cred' : 'bg-white bg-opacity-[5%] hover:text-cred'">
        <p class="h-min w-full">{{ text }}</p>
    </div>
</template>