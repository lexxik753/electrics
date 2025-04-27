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
    <header class="flex bg-[#18212b] text-white">
        <div class="flex m-auto">
            <img src="../assets/media/logo.png" alt="логотип электромонтажа">
        </div>
        <nav class="flex grow md:items-center">
            <ul class="hidden md:flex lg:flex-row">
                <li class="px-6" v-for="(link, index) in menu" :key="index"><a :href="link.link">{{ link.title }}</a>
                </li>
            </ul>
            <button class="md:hidden ml-auto mr-3">
                <svg class=" hover:stroke-2" width="32" height="32" viewBox="0 0 32 32" fill="none"
                    xmlns="http://www.w3.org/2000/svg" stroke="white">
                    <path d="M6 9.99927L26 9.99978" />
                    <path d="M6 15.9998L26 16.0003" />
                    <path d="M6 22.0002L26 22.0008" />
                </svg>
            </button>
        </nav>
    </header>
</template>
