<script setup>
import ServicesDetails from '../components/ServicesDetails.vue';

const servicesDetails = [
    {
        title: 'Замена автоматов',
        price: 'от 250₽',
    },
    {
        title: 'Замена проводки',
        price: 'от 250₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Диагностика проводки',
        price: 'от 1500₽',
    },
    {
        title: 'Установка розеток и выключателей',
        price: 'от 350₽',
    },
    {
        title: 'Ремонт розеток и выключателей',
        price: 'от 300₽',
    },
    {
        title: 'Установка автоматов защиты',
        price: 'от 250₽',
    },
    {
        title: 'Ремонт люстр и осветительных приборов',
        price: 'от 1000₽',
    },
    {
        title: 'Демонтаж люстры',
        price: 'от 300₽',
    },
    {
        title: 'Аварийный вызов электрика',
        price: 'от 1000₽'
    },
    {
        title: 'Расчёт и распределение нагрузки на кабель',
        price: 'от 100₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Установка генераторов',
        price: 'от 500₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Установка стабилизаторов напряжения',
        price: 'от 250₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Замена трансформаторов тока',
        price: 'от 300₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Перенос розеток',
        price: 'от 500₽'
    },
    {
        title: 'Установка розетки для электроплиты',
        price: 'от 1000₽'
    },
    {
        title: 'Установка бра',
        price: 'от 500₽'
    },
    {
        title: 'Установка светодиодной ленты',
        price: 'от 500₽'
    },
    {
        title: 'Установка точечного светильника',
        price: 'от 300₽'
    },
    {
        title: 'Установка люстр и потолочных светильников',
        price: 'от 1000₽'
    },
    {
        title: 'Демонтаж бра',
        price: 'от 150₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Замена ламп',
        price: 'от 50₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Подключение электрических духовых шкафов',
        price: 'от 500₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Проект квартиры, консультации по ремонту квартир',
        price: 'от 1500₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Монтаж электрического тёплого пола',
        price: 'от 1500₽'
    },
    {
        title: 'Установка звонка',
        price: 'от 200₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Демонтаж электросети',
        price: 'от 100₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Установка электросчётчика',
        price: 'от 500₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Сборка электрощита',
        price: 'от 1000₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Замена приборов учёта',
        price: 'от 500₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Подключение силового кабеля к щиту',
        price: 'от 250₽*',
        clarification: '*Уточняйте стоимость работ'
    },
    {
        title: 'Установка распределительных коробок',
        price: 'от 150₽*',
        clarification: '*Уточняйте стоимость работ'
    },
]

</script>

<template>
    <section class="container mt-15 mx-auto md:px-4">
        <div class="text-center pb-6">
            <h2 class="mb-2 text-xl md:text-2xl lg:text-4xl font-bold">Услуги, которые работают</h2>
            <p class="text-base lg:text-lg xl:text-2xl">Наша команда занимается электромонтажом и предлагает техническое
                обслуживание, ремонт и консультации для стабильной работы систем</p>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-3 items-stretch gap-2 divide-y lg:divide-y-0 lg:divide-x-2">
            <ServicesDetails :details="servicesDetails" />
        </div>
    </section>
</template>