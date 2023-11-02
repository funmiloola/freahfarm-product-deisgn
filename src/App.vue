<template>
  <div id="app">
   <header-section/>
  </div>
</template>

<script>
 import HeaderSection from "./components/HeaderSection.vue";
 
export default {
  name: 'App',
  components: {
    HeaderSection,

  }
}
</script>

<style scoped>
 #app{
  width:1440px;
 }
</style>
