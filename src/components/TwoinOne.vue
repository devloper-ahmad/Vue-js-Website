

<script setup>
import {defineProps } from 'vue'
const props = defineProps(['name','imgsrc','visit','btnName'])
</script>

<template>
  
    
    <section id="home"  class="py-5  bg-[#171c5d]">
  <div class="container flex flex-wrap items-center justify-center mx-auto mt-10 md:px-12 md:flex-row">
  <div class="1g:mb-0 1g:w-1/2">
  <h1 class="max-w-xl lg:text-[2.9rem] leading-none text-white font-extrabold font-sans text-center sm:text-base md:text-6xl lg:text-6xl
  lg:text-left lg:leading-tight mb-5">
  {{name}}
  </h1>
  <p class="max-w-xl text-center text-[#6c72ae] lg:text-lg lg:font-4xl lg:text-left lg:max-w-md">
    Moderne provides highly tailored ad ideas and insights, offering a digital workspace for more effective brainstorming for creative minds
  </p>
  <div class="flex justify-center mt-14 lg:justify-start">
    <router-link :to="visit" class="text-white bg-[#ff7e85] font-medium  px-20 py-5 text-2xl rounded-sm text-center
  hover:bg-indigo-500 hover: drop-shadow-md transition duration-300 ease-in-out">{{ btnName }}</router-link>

   </div>
  </div>
  <div class=" home lg:w-1/2 md:w-1 ">
  <img :src="imgsrc" class="sm:h-[100px;]  md:ml-8 md:h-[80%] md:w-[80%]"  alt="hero-img">
  </div>
  </div>
  </section>
 
  
  
</template>

<style scoped>
.home{
  animation: up-down 1s alternate infinite;
}
@keyframes up-down{
  0%{

    transform: translateY(10px);
  }
  100%{
    transform: translateY(-10px);
  }
}
</style>