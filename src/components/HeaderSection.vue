<template>
  <div>
  <nav>
    <div class="nav-section">
      <img src="@/assets/images/FreshFarm.svg" alt="" class="logo" />
    </div>
    <ul>
      <li v-for="(nav, index) in navs" :key="index" class="options">
        {{ nav }}
      </li>
    </ul>
    <div class="nav-btns">
      <button class="login-btn">Login</button>
      <button class="order-btn">Order Now</button>
    </div>
    <div class="nav-icon" @click="toggleIcon">
      <img src="@/assets/images/icon-menu.svg" alt="" id="icon-menu" v-if="showIcon" >
      <img src="@/assets/images/icon-close.svg" alt="" id="icon-close" v-else>
    </div>
  </nav>
  <side-bar v-if="showSidebar"/>
  </div>
</template>

<script>
import SideBar from "@/components/SideBar.vue";
export default {
  components: {
    SideBar
  },
  data() {
    return {
      navs: ["Home", "About", "Contact Us", "Testimonials"],
      showIcon:true,
      showSidebar:false,
      iconSource:[require('@/assets/images/icon-menu.svg'),require('@/assets/images/icon-close.svg')]
    };
  },
  methods:{
    toggleIcon(){
      this.showIcon =! this.showIcon;
      this.showSidebar =! this.showSidebar;
    }
  }
};
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Commissioner:wght@400;500;700&family=DM+Sans:opsz,wght@9..40,400;9..40,500&family=Inter:wght@400;500;700&family=Josefin+Sans:wght@400;700&family=Karla:wght@400;700&family=Kumbh+Sans:wght@400;700&family=League+Spartan:wght@500;700&family=Lexend+Deca&family=Manrope:wght@800&family=Pacifico&family=Plus+Jakarta+Sans:wght@500;800&family=Roboto:wght@400;700&display=swap');
* {
  padding: 0;
  margin: 0;
}
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width:1280px;
  margin:0 auto;
  padding-top:20px;
  padding-bottom:20px;
}
ul {
  display:flex;
  gap:50px;
}
@media (max-width:992px){
  ul{
    display:none;
  }
}
 ul li {
  list-style-type: none;
  font-family: inter;
  font-weight: 500;
  font-size: 18px;
  cursor:pointer;
}
@media(max-width:992px){
.logo {
   width:200px;
   padding-left:4px;
}
}

.nav-btns{
  display: flex;
  align-items: center;
  gap: 32px;
}
@media(max-width:992px){
  .nav-btns{
    display: none;
  }
}
.login-btn {
  font-family: inter;
  font-weight: 500;
  color:#000;
  font-size:18px;
  background: transparent;
  border:none;
}
.order-btn {
  padding: 20px 45px 20px 45px;
  background: #008000;
  color: #fff;
  border: none;
  border-radius: 8px;
  font-size: 18px;
  font-weight: 700;
  font-family: inter;
}
#icon-menu{
  width:34px;
}
#icon-close{
  width:34px;
}
.nav-icon{
  display:none;
}
@media(max-width:992px){
  .nav-icon{
    display:block;
    padding-right:0.5rem;
  }
}
</style>