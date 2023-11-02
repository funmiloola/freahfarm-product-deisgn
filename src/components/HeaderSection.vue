<template>
  <div>
    <nav>
        <ul class="nav-section">
        <li class="freshfarm-logo">FreshFarm</li>
        <li class="options">Home</li>
        <li  class="options">About</li>
        <li  class="options">Contact Us</li>
        <li  class="options">Testimonials</li>
        </ul>
        <ul class="nav-options">
            <li class="login">Login</li>
            <li><button>Order Now</button></li>
        </ul>
    </nav>
  </div>
</template>

<script>

export default {

}
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Commissioner:wght@400;500;700&family=DM+Sans:opsz,wght@9..40,400;9..40,500&family=Inter&family=Josefin+Sans:wght@400;700&family=Karla:wght@400;700&family=Kumbh+Sans:wght@400;700&family=League+Spartan:wght@500;700&family=Lexend+Deca&family=Manrope:wght@800&family=Pacifico&family=Plus+Jakarta+Sans:wght@500;800&family=Roboto:wght@400;700&display=swap');
 *{
  padding:0;
  margin:0;
 }
 nav{
  display:flex;  
  gap:154px;
 }
 ul{
  
 }
 li{
  list-style-type: none;
  
 }
.freshfarm-logo{
  font-family: Pacifico;
  font-weight:400;
  font-size:48px;
  color:#008000;
  padding-left:121px;
}
.nav-section{
  display: flex;
  align-items:center;
}
.options{
  font-family:inter;
  font-weight:500;
  font-size:18px;
  padding-left:52px;
} 
.nav-options{
  display:flex;
  align-items:center;
  gap:32px;
}
.login{
  font-family: inter;
  font-weight: 500;
  font-size: weight;
}
button{
  padding:20px 75px 20px 75px;
  background:#008000;
  color:#fff;
  border:none;
  border-radius:8px;
  font-size:18px;
  font-weight:700;
  font-family:inter;
}
</style>