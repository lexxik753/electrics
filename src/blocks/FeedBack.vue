<script setup>
import FeedbackForm from '../components/FeedbackForm.vue';
</script>

<template>
    <section class="container mt-15 mx-auto px-4">
        <div class="text-center">
            <h3 class="mb-5 mx-auto text-xl md:text-2xl lg:text-4xl font-bold">Свяжитесь с нами</h3>
            <p class="mb-3 mx-auto text-base lg:text-lg xl:text-xl">Мы оперативно ответим на ваш запрос по телефону или электронной почте.</p>
        </div>
        <div>
            <FeedbackForm />
        </div>
    </section>
</template>