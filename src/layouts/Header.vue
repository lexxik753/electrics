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
    <header class="bg-neutral-100 py-4 flex">
        <div class="flex items-center">
            <img class="mx-1" src="../assets/media/logo.png" alt="логотип электромонтажа">
            <h1 class="ml-1 text-2xl uppercase">Электромонтаж</h1>
        </div>
        <nav class="pl-4 flex items-center">
            <ul class="flex">
                <li class="px-6" v-for="(link, index) in menu" :key="index"><a :href="link.link">{{ link.title }}</a></li>
            </ul>
        </nav>
    </header>
</template>
