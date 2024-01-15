<script setup>
    const props = defineProps(['title', 'des'])
</script>

<template>
    <div class="exp-card-wrapper p-4 h-36">
        <div class="bg-black rounded-[8px] h-full">
            <div class="py-4 px-2 lg:p-4 bg-white bg-opacity-[5%] transition-all duration-300 hover:bg-opacity-[10%] exp-card">
                <h1 class="text-[32px] lg:text-[36px] stix">{{ title }}</h1>
                <p class="text-[14px] lg:text-[16px] text-cgray">{{ des }}</p>
            </div>
        </div>
    </div>
</template>