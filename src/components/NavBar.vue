<script setup>
import { RouterLink } from 'vue-router';
</script>

<template>
  

<nav class="Nav bg-[#171c5d] border-gray-200 ">
  <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-10">
  <a href="#" class="flex items-center space-x-3 rtl:space-x-reverse">
      <img src="../assets/images/icon-cols-0.png" class="h-8" alt="Flowbite Logo" />
      <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">Moderne</span>
  </a>
  <div class="flex md:order-2 space-x-3 md:space-x-0 rtl:space-x-reverse">
      <button type="button" class="text-[#060e60] bg-[#f6c8f1] hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-sm text-sm px-10 py-3 font-serif text-center  dark:hover:bg-blue-700 dark:focus:ring-blue-800">Get a Demo</button>
      <button data-collapse-toggle="navbar-cta" type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-cta" aria-expanded="false">
        <span class="sr-only">Open main menu</span>
        <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>
        </svg>
    </button>
  </div>
  <div class="items-center justify-between ml-36 hidden w-full md:flex md:w-auto md:order-1" id="navbar-cta">
    <ul class="flex flex-col font-medium p-4 md:p-0 mt-9 md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0 md:border-0">
      <li>
        <!-- <router-link to="/" class="block py-2 text-lg px-3 md:p-0 text-white bg-blue-700 rounded md:bg-transparent md:text-blue-700 md:dark:text-blue-500" aria-current="page">Home</router-link> -->
        <router-link to="/" v-slot="{ isActive }">
      <a
        :class="[
          'block py-2 text-lg px-3 md:p-0 rounded',
          isActive 
            ? 'text-white bg-blue-700 md:bg-transparent md:text-blue-700 md:dark:text-blue-500'
            : 'text-gray-700 md:text-gray-500 md:dark:text-gray-400'
        ]"
        aria-current="page"
      >
        Home
      </a>
    </router-link>
      </li>
      <li>
        <router-link to="/about" v-slot="{ isActive }">
      <a
        :class="[
          'block py-2 text-lg px-3 md:p-0 rounded',
          isActive 
            ? 'text-white bg-blue-700 md:bg-transparent md:text-blue-700 md:dark:text-blue-500'
            : 'text-gray-700 md:text-gray-500 md:dark:text-gray-400'
        ]"
        aria-current="page"
      >
        About
      </a>
    </router-link>
      </li>
      <li>
        <router-link to="/Services" v-slot="{ isActive }">
      <a
        :class="[
          'block py-2 text-lg px-3 md:p-0 rounded',
          isActive 
            ? 'text-white bg-blue-700 md:bg-transparent md:text-blue-700 md:dark:text-blue-500'
            : 'text-gray-700 md:text-gray-500 md:dark:text-gray-400'
        ]"
        aria-current="page"
      >
        Services
      </a>
    </router-link>
      </li>
      <li>
        <router-link to="/Page" v-slot="{ isActive }">
      <a
        :class="[
          'block py-2 text-lg px-3 md:p-0 rounded',
          isActive 
            ? 'text-white bg-blue-700 md:bg-transparent md:text-blue-700 md:dark:text-blue-500'
            : 'text-gray-700 md:text-gray-500 md:dark:text-gray-400'
        ]"
        aria-current="page"
      >
        Page
      </a>
    </router-link>
      </li>
      <li>
        <router-link to="/Pricing" v-slot="{ isActive }">
      <a
        :class="[
          'block py-2 text-lg px-3 md:p-0 rounded',
          isActive 
            ? 'text-white bg-blue-700 md:bg-transparent md:text-blue-700 md:dark:text-blue-500'
            : 'text-gray-700 md:text-gray-500 md:dark:text-gray-400'
        ]"
        aria-current="page"
      >
        Pricing
      </a>
    </router-link>
      </li>
      <li>
        <router-link to="/Login" v-slot="{ isActive }">
      <a
        :class="[
          'block py-2 text-lg px-3 md:p-0 rounded',
          isActive 
            ? 'text-white bg-blue-700 md:bg-transparent md:text-blue-700 md:dark:text-blue-500'
            : 'text-gray-700 md:text-gray-500 md:dark:text-gray-400'
        ]"
        aria-current="page"
      >
        Login
      </a>
    </router-link>
      </li>
    </ul>
  </div>
  </div>
</nav>

  
</template>

<style  scoped>
.isActive {
  font-weight: bold;
  color: red;
}
</style>