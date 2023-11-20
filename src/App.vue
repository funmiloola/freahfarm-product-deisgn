<template>
  <div id="app">
   <header-section/>
    <hero-section/> 
   <service-section/>
    <about-section/>
   <food-category/>
   <special-dishes/>
   <review-section/> 
   <footer-section/>
  </div>
</template>

<script>
 import HeaderSection from "./components/HeaderSection.vue";
 import HeroSection from "./components/HeroSection.vue";
 import ServiceSection from "./components/ServiceSection.vue";
 import AboutSection from "./components/AboutSection.vue";
 import FoodCategory from "./components/FoodCategory.vue";
 import SpecialDishes from "./components/SpecialDishes.vue";
 import ReviewSection from "./components/ReviewSection.vue";
 import FooterSection from "./components/FooterSection.vue";
export default {
  name: 'App',
  components:{
    HeaderSection,
    HeroSection,
    ServiceSection,
    AboutSection,
    FoodCategory,
    SpecialDishes,
    ReviewSection,
    FooterSection
  }
}
</script>

<style scoped>
 
</style>
