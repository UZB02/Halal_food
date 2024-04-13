<template>
  <header class="w-full">
    <nav class="bg-white w-full border-gray-200 shadow dark:bg-gray-900">
  <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto">
  <a href="https://flowbite.com/" class="flex items-center justify-center space-x-3 rtl:space-x-reverse">
      <img src="https://sun9-46.userapi.com/impf/c628817/v628817094/29177/0GA771Ypp3A.jpg?size=585x604&quality=96&sign=a611e45b60ac0f8e79c4211679d87e38&type=album" class="w-16 rounded-s-full" alt="Flowbite Logo" />
      <h2 class="self-center text-3xl font-bold whitespace-nowrap dark:text-white">Halal Food</h2>
  </a>
     <button @click="toggle"  type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600">
        <span class="sr-only">Open main menu</span>
        <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>
        </svg>
    </button>
  <div :class="active ? 'items-center justify-between absolute top-12 block w-full md:flex md:w-auto md:order-1' : 'items-center justify-between hidden w-full md:flex md:w-auto md:order-1'" >
    <ul class="flex flex-col font-medium p-4 md:p-0 mt-4 border border-gray-100  bg-gray-50 md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0 md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700">
      <li>
        <a href="#" class="block py-2 px-3 md:p-0 text-white bg-blue-700 rounded md:bg-transparent md:text-blue-700 md:dark:text-blue-500" aria-current="page">Home</a>
      </li>
      <li>
        <a href="#" class="block py-2 px-3 md:p-0 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">About</a>
      </li>
      <li>
        <a href="#" class="block py-2 px-3 md:p-0 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">Services</a>
      </li>
      <li>
        <a href="#" class="block py-2 px-3 md:p-0 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">Contact</a>
      </li>
    </ul>
  </div>
  </div>
</nav>
  </header>
  <section id="page1" class="w-full flex items-center justify-center h-[90.5vh]">
    <div class="container w-[1200px] flex items-center h-full">
      <span class="flex flex-col gap-3 w-1/2 max-[380px]:w-full max-[380px]:items-center">
     <span class=" flex gap-2"><h1 class="text-5xl max-[380px]:text-3xl font-bold text-white">Welcome to <h1 class="text-5xl max-[380px]:text-3xl font-bold text-lime-400">Halal Food</h1></h1></span>
      <p class="text-white max-[380px]:text-base max-[380px]:text-center">Korreadagi mijozlarimiz uchun menusi faqat musulmon halol taomlaridan iborat bo'lgan <span class="text-lime-400">HALAL FOOD</span> markazimiz 12.12.2023 dan siz yaqinlarimiz uchun halol taomlarni taqdim etadi</p>
      </span>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';

const active = ref(false);

const toggle = () => {
  active.value = !active.value
  console.log(active.value);
}

</script>

<style scoped>
#page1{
  background: url('https://rare-gallery.com/uploads/posts/1218448-mandala.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  object-fit: cover;
}
</style>
