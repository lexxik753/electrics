<script setup>
const props = defineProps({
    details: [
        {
            title: String,
            price: String,
            descriptions: String
        }
    ],
})
</script>

<template>
    <div v-for="(detail, index) in props.details" :key="index" class="mt-4 py-3 flex justify-center space-x-8">
        <h3 class="text-lg font-bold mb-4 pb-1 border-b-2 border-orange-500 inline-block">{{ detail.title }}</h3>
        <p>{{ detail.price }}</p>
    </div>
</template>