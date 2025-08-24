<script setup>
import FeedbackForm from '../components/FeedbackForm.vue';
</script>

<template>
    <section class="container mt-15 mx-auto px-4">
        <h3 class="pb-5 text-xl md:text-2xl lg:text-4xl text-center font-bold">Свяжитесь с нами</h3>
        <p class="text-center lg:text-2xl/relaxed md:text-xl/loose ">
            Мы оперативно ответим на ваш запрос по телефону или электронной почте.
        </p>
        <div>
            <FeedbackForm />
        </div>
    </section>
</template>