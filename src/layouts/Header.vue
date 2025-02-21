<script setup>
import { ref } from 'vue';

const menu = ref([
    {
        title: 'О компании',
        link: '#',
    },
    {
        title: 'Проекты',
        link: '#',
    },
    {
        title: 'Услуги',
        link: '#',
    },
    {
        title: 'Отзывы',
        link: '#',
    },
    {
        title: 'Контакты',
        link: '#',
    },
])
</script>
<template>
    <header class="bg-zinc-300 py-4 flex">
        <div class="flex items-center">
            <img src="../assets/media/logo.png" alt="">
            <h1 class="ml-1 text-2xl uppercase">Электромонтаж</h1>
        </div>
        <nav class=" flex items-center grow">
            <ul class="flex grow">
                <li v-for="(link, index) in menu" :key="index"><a :href="link.link">{{ link.title }}</a></li>
            </ul>
        </nav>
    </header>
</template>
