<script setup lang="ts">

</script>

<template>
    <div>
        
    <div class="flex flex-wrap justify-center space-x-4 p-4  bg-[#f3eae5]" >
    <div v-for="n in 15"
      :key="n"
      class="bg-white shadow-md rounded-lg overflow-hidden w-64 m-2 transform transition-transform duration-500 hover:rotate-6 hover:scale-105" >
      <div class="p-4 mt-6">
        <p class="text-gray-700 text-base mb-4">
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante."
        </p>
        <div class="flex items-center mb-4">
          <img class="w-12 h-12 rounded-full mr-4" :src="'https://i.pravatar.cc/150?img=' + n" alt="Avatar">
          <div class="text-sm">
            <p class="text-gray-900 leading-none">Person {{ n }}</p>
            <p class="text-gray-600">Position {{ n }}</p>
          </div>
        </div>
        <button class="bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-600 focus:outline-none opacity-0 hover:opacity-100 transition-opacity duration-500">
          More Info
        </button>
      </div>
    </div>
  </div>
    </div>
</template>

<style lang="css" scoped>

</style>