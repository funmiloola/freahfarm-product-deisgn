<template>
  <div>
    <div class="sidebar">
        <ul>
      <li v-for="(nav, index) in navs" :key="index" class="options">
        {{ nav }}
      </li>
    </ul>
    <div class="nav-btns">
      <button class="login-btn">Login</button>
      <button class="order-btn">Order Now</button>
    </div>
    </div>
  </div>
</template>

<script>
 
 
export default {
     data(){
        return{
            navs: ["Home", "About", "Contact Us", "Testimonials"]
        }
     }
}
</script>

<style scoped>
 *{
    padding:0;
    margin:0;
 }
 ul li{ 
    list-style-type: none;
    text-align: center;
    padding-top:2rem;
    font-family: inter;
    font-weight: 500;
    font-size: 18px;
    cursor:pointer;
 }
 .sidebar{
    display:none;
 }
 @media (max-width:992px){
.sidebar{
    padding:0;
     display: flex;
     flex-direction: column;
     gap:2rem;
     position: fixed;
     background: #fff;
     width:100vw;
     height: 100%;
     left:0
     
}
 }
 .nav-btns{
    display:flex;
    flex-direction: column;
    align-items: center;
    gap:2rem;
 }
 .login-btn{
    font-family: inter;
    font-weight: 500;
    color:#000;
    font-size:18px;
    background: transparent;
    border:none;
 }
.order-btn{
    padding: 15px 75px 15px 75px;
    background: #008000;
    color: #fff;
    border: none;
    border-radius: 8px;
    font-size: 18px;
    font-weight: 700;
    font-family: inter;
}
</style>
