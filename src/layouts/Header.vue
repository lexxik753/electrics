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

const showMenu = ref(false);

</script>
<template>
    <header class="flex bg-[#18212b] text-white">
        <nav class="flex grow items-center md:flex md:grow md:items-center">
            <div>
                <img class="m-auto" src="../assets/media/logo.png" alt="логотип электромонтажа">
            </div>
            <ul class="hidden md:flex lg:flex-row">
                <li class="px-6" v-for="(link, index) in menu" :key="index"><a :href="link.link">{{ link.title }}</a>
                </li>
            </ul>
        </nav>
        <button class="block md:hidden ml-auto mr-3 relative" @click="showMenu = true">
            <svg class=" hover:stroke-2" width="32" height="32" viewBox="0 0 32 32" fill="none"
                xmlns="http://www.w3.org/2000/svg" stroke="white">
                <path d="M6 9.99927L26 9.99978" />
                <path d="M6 15.9998L26 16.0003" />
                <path d="M6 22.0002L26 22.0008" />
            </svg>
        </button>
        <div class="bg-[#18212b] md:hidden h-[100vh] w-full absolute top-0"
            :class="showMenu == true ? 'block' : 'hidden'">
            <div class="flex justify-end mt-4 mr-5">
                <button @click="showMenu = false">X</button>
            </div>
            <ul class="flex flex-col items-center space-y-2 ">
                <li class="px-6" v-for="(link, index) in menu" :key="index"><a :href="link.link">{{ link.title }}</a>
                </li>
            </ul>
        </div>
    </header>
    <div
        class="min-h-screen bg-[url('./assets/media/bg-header.png')] bg-cover text-white relative before:absolute before:inset-0 before:bg-gradient-to-r before:from-black/70 before:to-transparent">
        <div class="relative z-10">
            <h2 class="py-4 text-xl md:text-2xl text-center">ЭЛЕКТРОМОНТАЖ</h2>
            <h1 class="mb-4 text-2xl md:text-[52px] font-bold text-center">Электричество для вашего дома</h1>
            <section class="m-auto w-1/2 text-center">
                <p class="md:text-lg md:leading-loose">Мы предлагаем комплексные решения в области электротехники и
                    сантехники,
                    учитывая ваши индивидуальные потребности. От начальной установки до регулярного обслуживания, мы
                    гарантируем профессионализм и качественную работу, которой вы можете доверять.</p>
            </section>
        </div>
    </div>
</template>
