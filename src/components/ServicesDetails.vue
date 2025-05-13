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
<!-- last:col-span-3 last:justify-center  -->
<template>
    <div v-for="(detail, index) in props.details" :key="index" class="mt-4 p-3 flex justify-between items-baseline space-x-5">
        <h3 class="text-lg font-bold mb-4 pb-1 border-b-2 border-orange-500 inline-block">{{ detail.title }}</h3>
        <p>{{ detail.price }}</p>
    </div>
</template>