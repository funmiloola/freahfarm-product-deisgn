<template>
  <div id="app">
   <header-section/>
   <hero-section/>
  </div>
</template>

<script>
 import HeaderSection from "./components/HeaderSection.vue";
 import HeroSection from "./components/HeroSection.vue"
export default {
  name: 'App',
  components: {
    HeaderSection,
    HeroSection
  }
}
</script>

<style scoped>
 
</style>
