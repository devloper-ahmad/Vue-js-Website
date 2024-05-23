<script setup>

import TwoinOne from '../components/TwoinOne.vue'
import home from '../assets/images/hero-monkey.png';
import Page from '../components/Page.vue'


</script>

<template>
  
    <TwoinOne :name="'Unleash the full potential of your creative team'" :imgsrc="home" :visit="'/about'" :btnName="'Get Started'"/>
   
    <Page/>
    
    </template> 
    
<style>

</style> 