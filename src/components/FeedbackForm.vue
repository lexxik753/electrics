<script setup>

</script>
<template>
    <div class="mt-4 ">
        <form action="" class="p-10 grid grid-cols-3 gap-3 w-full lg:w-2/3 sm:place-self-center shadow-2xl">
            <input type="text" name="userEmail" placeholder="Ваш электронный адрес" class="mb-2 p-4 border-2 border-gray-300 bg-blue-100" />
            <input type="text" name="userPhone" placeholder="Ваш номер телефона" class="mb-2 p-4 border-2 border-gray-300 bg-blue-100" />
            <input type="text" name="userName" placeholder="Ваше полное имя" class="mb-2 p-4 border-2 border-gray-300 bg-blue-100" />
            <textarea type="text" name="userComments" placeholder="Ваши комментарии" class="p-4 col-span-3 border-2 border-gray-300 bg-blue-100" />
            <button class="my-2 p-3 w-1/2 rounded-full bg-blue-400">Оставить заявку</button>
        </form>
    </div>
</template>
