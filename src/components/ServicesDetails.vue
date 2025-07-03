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
    <div 
        v-for="(detail, index) in props.details" 
        :key="index"
        class="h-full px-2 flex flex-col md:flex-wrap justify-between items-baseline">
        <div class="flex-grow">
            <p class="text-xs md:text-base font-bold mb-2 border-b-2 border-orange-500">{{ detail.title }}</p>
            <p class="text-xs md:text-base">{{ detail.price }}</p>
            <p class="w-full pt-1 text-xs text-gray-700">{{ detail.clarification }}</p>
        </div>
    </div>
</template>