<script setup>

</script>
<template>
    <div class="mt-4 flex flex-col md:grid grid-cols-2 grid-rows-1  gap-7">
        <p class="place-self-center-safe text-center lg:text-2xl/relaxed md:text-xl/loose ">
            Мы оперативно ответим на ваш запрос по телефону или электронной почте.
        </p>
        <div>
            <form action="" class="flex flex-col w-full lg:w-2/3 sm:place-self-center">
                <input type="text" name="userEmail" placeholder="Ваш электронный адрес" class="mb-2 p-4 border-2 border-gray-300 bg-blue-100" />
                <input type="text" name="userPhone" placeholder="Ваш номер телефона" class="mb-2 p-4 border-2 border-gray-300 bg-blue-100" />
                <input type="text" name="userName" placeholder="Ваше полное имя" class="mb-2 p-4 border-2 border-gray-300 bg-blue-100" />
                <textarea type="text" name="userComments" placeholder="Ваши комментарии" class="p-4 border-2 border-gray-300 bg-blue-100" />
                <button class="my-2 p-3 w-1/2 rounded-full bg-blue-400">Оставить заявку</button>
            </form>
        </div>
    </div>
</template>
