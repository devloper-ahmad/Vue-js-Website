<script setup >


import cards from '../components/cards.vue'
import Services from '../components/Services.vue'
import testomonial from './testomonial.vue'
</script>



<template>
    <div class="Page bg-[#f3eae5]">
        <section class="text-gray-600  body-font">
     
  <div class="container px-5  mx-auto flex flex-wrap">
    <div class="lg:w-1/2 w-full mb-10 lg:mb-0 rounded-lg overflow-hidden">
      <img alt="feature" class="object-cover object-center lg:h-[488px;] sm:h-[200px;]" src="../assets/images/features-01.png">
    </div>
    <div class="flex flex-col flex-wrap lg:py-6 -mb-10 lg:w-1/2 lg:pl-12 lg:text-left text-center">
      <div class="flex flex-col mb-10 lg:items-start items-center">
       
        <div class="flex-grow">
          
          <h1 class="leading-relaxed lg:text-6xl md:text-6xl sm:text-lg text-[#0e1889] font-bold">Thousands of insights, trends and ideas</h1>
            <p class=" text-lg mt-3">Moderne collects thousands of trends, innovative ideas and advertising campaigns from all over the world and extracts consumer, market and inspiration insights and then selects them based on your goals & objectives, target audience and data.</p>
        
            <button class="bg-yellow-500 hover:bg-yellow-900 text-white font-bold text-2xl md:py-2 px-16 py-4 rounded  mt-4">Read More</button>
        </div>
      </div>   
    </div>
  <div class=" px-5  flex flex-wrap ">
  <div class="flex flex-col flex-wrap lg:py-6 mb-10 lg:w-1/2 lg:pl-12 lg:text-left text-center">
      <div class="flex flex-col mb-10 lg:items-start items-center">

        <div class="flex-grow ">
          
          <h1 class="leading-relaxed lg:text-6xl md:text-6xl  sm:text-lg text-[#0e1889] font-bold">Thousands of insights, trends and ideas</h1>
            <p class="text-lg mt-3">Moderne collects thousands of trends, innovative ideas and advertising campaigns from all over the world and extracts consumer, market and inspiration insights and then selects them based on your goals & objectives, target audience and data.</p>
        
            <button class="bg-yellow-500 hover:bg-yellow-900 text-white font-bold text-2xl md:py-2 px-16 py-4 rounded  mt-4">Read More</button>
        </div>
      </div>
    </div>
    
    <div class="lg:w-1/2 w-full mb-10 lg:mb-0 rounded-lg overflow-hidden">
      <img alt="feature" class="object-cover object-center lg:h-[488px;] sm:h-[200px;] lg:ml-11" src="../assets/images/features-02.png">
    </div>
  
  
<div class="paragraph mt-24 ml-16">
  <div class="tex">
    <h1 class="para lg:text-4xl font-semi-bold tracking-wide font-serif">
      Moderne helps creative teams to <span>save  <br> hours or even days</span> on research and allows <br>
       them to collaborate <span>up to 3x faster</span> 
</h1>
</div>


<cards/>


</div>
  </div>
  </div>
  
  <services/>
  <testomonial class="mt-5"/>

</section> 

    </div>
</template>

<style  scoped>
span{

  color: #dd59cf;
}
</style>