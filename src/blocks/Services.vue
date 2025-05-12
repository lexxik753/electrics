<script setup>
import ServicesDetails from '../components/ServicesDetails.vue';

const servicesDetails = [
    {
        title: 'Электромонтажные работы',
        price: 'от 500₽',
    },
    {
        title: 'Ремонт',
        price: 'от 500₽',
    },
    {
        title: 'Комплексные электромонтажные работы',
        price: 'Договорная',
    },
    {
        title: 'Электромонтажные работы',
        price: 'от 500₽',
    },
    {
        title: 'Ремонт',
        price: 'от 500₽',
    },
    {
        title: 'Комплексные электромонтажные работы',
        price: 'Договорная',
    },
]

</script>

<template>
    <section class="container mt-15 mx-auto px-4">
        <div class="text-center">
            <h2 class="mb-2 text-xl md:text-2xl lg:text-4xl font-bold">Услуги, которые работают</h2>
            <p class="text-base lg:text-lg xl:text-2xl">Наша команда занимается электромонтажом и предлагает техническое
                обслуживание, ремонт и консультации для стабильной работы систем</p>
        </div>
        <div class="grid grid-cols-3 divide-x-2">
            <ServicesDetails :details="servicesDetails"/>
            <!-- <ServicesDetails/>
            <ServicesDetails/> -->
        </div>
    </section>
</template>