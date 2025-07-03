<script setup>
const props = defineProps({
    details: [
        {
            title: String,
            price: String,
            clarification: String
        }
    ],
})
</script>
<template>
    <div v-for="(detail, index) in props.details" :key="index" class="mt-4 p-2 flex flex-wrap justify-between items-baseline">
        <p class="text-sm md:text-base font-bold mb-4 pb-1 border-b-2 border-orange-500 inline-block">{{ detail.title }}</p>
        <p>{{ detail.price }}</p>
        <p class="w-full text-xs">{{ detail.clarification }}</p>
    </div>
</template>