<template>
  <nav>
    <div class="nav-section">
      <li class="freshfarm-logo">FreshFarm</li>
      <!-- <img src="" alt="" /> -->
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
  </nav>
</template>

<script>
export default {
  data() {
    return {
      navs: ["Home", "About", "Contact Us", "Testimonials"],
    };
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Commissioner:wght@400;500;700&family=DM+Sans:opsz,wght@9..40,400;9..40,500&family=Inter&family=Josefin+Sans:wght@400;700&family=Karla:wght@400;700&family=Kumbh+Sans:wght@400;700&family=League+Spartan:wght@500;700&family=Lexend+Deca&family=Manrope:wght@800&family=Pacifico&family=Plus+Jakarta+Sans:wght@500;800&family=Roboto:wght@400;700&display=swap");
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
 ul li {
  list-style-type: none;
  font-family: inter;
  font-weight: 500;
  font-size: 18px;
  cursor:pointer;
}
.freshfarm-logo {
  font-family: Pacifico;
  font-weight: 400;
  font-size: 48px;
  color: #008000;
  list-style-type: none;
}
.nav-section {
  display: flex;
  align-items: center;
}
.options {
   
  
}
.nav-btns{
  display: flex;
  align-items: center;
  gap: 32px;
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
</style>