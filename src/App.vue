<template>
  <div id="app">
   <header-section/>
   <hero-section/>
   <service-section/>
   <about-section/>
   <food-category/>
  </div>
</template>

<script>
 import HeaderSection from "./components/HeaderSection.vue";
 import HeroSection from "./components/HeroSection.vue";
 import ServiceSection from "./components/ServiceSection.vue";
 import AboutSection from "./components/AboutSection.vue";
 import FoodCategory from "./components/FoodCategory.vue" 
export default {
  name: 'App',
  components: {
    HeaderSection,
    HeroSection,
    ServiceSection,
    AboutSection,
    FoodCategory
  }
}
</script>

<style scoped>
 #app{
  width:1440px;
 }
</style>
