<script setup>

</script>
<template>
    <div class="mt-4 flex flex-col md:grid grid-cols-2 grid-rows-1 gap-7">
        <div class="place-self-center">
            <p>8 800 123-45-67</p>
            <p>example@example.ru</p>
            <p>Бизнес-центр «Прогресс», ул. 34, Москва</p>
        </div>
        <div>
            <form action="" class="flex flex-col w-2/3">
                <input type="text" name="userEmail" placeholder="Ваш электронный адрес" class="mb-2 p-4 border-2 border-gray-300 bg-blue-100"/>
                <input type="text" name="userName" placeholder="Ваше полное имя"  class="mb-2 p-4 border-2 border-gray-300 bg-blue-100"/>
                <input type="text" name="userComments" placeholder="Ваши комментарии" class="mb-2 p-4 border-2 border-gray-300 bg-blue-100"/>
                <button class="mb-2 p-4 w-1/2 rounded-full bg-blue-400">Оставить заявку</button>
            </form>
        </div>
    </div>
</template>
