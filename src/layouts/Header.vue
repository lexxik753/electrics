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
            <div class="w-32 md:w-40">
                <img class="w-full h-auto object-contain m-auto" src="../assets/media/logo.png"
                    alt="логотип электромонтажа" width="160" height="48">
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
        <div class="fixed inset-0 bg-[#18212b] md:hidden w-full z-50" :class="showMenu == true ? 'block' : 'hidden'">
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
        class="min-h-screen bg-[url('./assets/media/bg-header.png')] bg-cover text-white relative before:absolute before:inset-0 before:bg-linear-to-r before:from-black/70 before:to-transparent">
        <div class="relative z-10 text-shadow-lg/50">
            <h2 class="py-4 text-xl md:text-2xl text-center">ЭЛЕКТРОМОНТАЖ</h2>
            <h1 class="mb-4 text-2xl md:text-[52px] font-bold text-center">Электричество для вашего дома</h1>
            <section class="m-auto md:w-1/2 text-center">
                <p class="text-sm md:text-lg md:leading-loose">Мы предлагаем комплексные решения в области
                    электротехники и
                    сантехники,
                    учитывая ваши индивидуальные потребности. От начальной установки до регулярного обслуживания, мы
                    гарантируем профессионализм и качественную работу, которой вы можете доверять.</p>
                <a href="#"
                    class="bg-[#FF6B35] text-white my-4 py-3 px-8 rounded-lg hover:bg-[#FF7F4D] transition-colors shadow-md hover:shadow-lg inline-flex items-center gap-2">
                    <svg 
                        class="w-5 h-5" 
                        fill="currentColor" 
                        viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"
                        aria-hidden="true">
                        <path d="M13 10h7l-9 13v-9H4l9-13v9Z"/>
                    </svg>
                    Узнать больше
                </a>
            </section>
        </div>
    </div>
</template>
