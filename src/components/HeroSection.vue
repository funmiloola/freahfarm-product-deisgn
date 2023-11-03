<template>
  <div class="hero-section">
    <div class="order">
    <h1>Just <span>Eat healthy</span> food to live a healthier Life</h1>
    <p>Enjoy a healthy life by eating healthy meals that have extraordinary flavors that make your life healthier for today and in the future</p>
    <div class="btn">
    <button>Order Now</button>
    </div>
    </div>
    <div class="image-section">
   <img src="@/assets/images/unsplash_xeTv9N2FjXA.svg">
    </div>
  </div>
</template>

<script>
export default {

}
</script>
 
<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Commissioner:wght@400;500;700&family=DM+Sans:opsz,wght@9..40,400;9..40,500&family=Inter:wght@400;500;700&family=Josefin+Sans:wght@400;700&family=Karla:wght@400;700&family=Kumbh+Sans:wght@400;700&family=League+Spartan:wght@500;700&family=Lexend+Deca&family=Manrope:wght@800&family=Pacifico&family=Plus+Jakarta+Sans:wght@500;800&family=Roboto:wght@400;700&display=swap');
*{
    margin:0;
    padding:0;
}
@media(max-width:992px){
    *{
        margin:0;
    }
}
 .hero-section{
    display:flex;
    max-width: 1280px;
    justify-content: space-between;
    align-items: center;
    gap:10px;
    margin:0 auto; 
 }
 @media (max-width:992px){
    .hero-section{
        /* max-width: 900px; */
        display:inline-block;
    }
 }
 h1{
    font-family:inter;
    font-weight:700;
    font-size:64px;
    width:518px;
    height:249px;
 }
 @media(max-width:992px){
    h1{    
        width:auto;
        height: auto;    
       text-align: center;
       font-size:56px;
       padding-top:16px;
    }
 }
span{
    color:#008000;
}
p{
    /* width:421px;
    height:98px; */
    font-family:inter;
    font-weight:500;
    font-size:20px;
    color:#3A3A3A;
    line-height:32.4px;
    padding-top:32px;
}
@media(max-width:992px){
    p{
      text-align: center; 
      font-size:16px;

    }
}
.btn{
    padding-top:32px;
}
button{
    padding:20px 45px 20px 45px;
    border:none;
    border-radius:8px;
    background:#008000;
    color:#fff;
    font-size:18px;
    font-family:inter;
    font-weight: 700;
}
@media(max-width:992px){
    .btn{
      display: flex;
      align-items: center;
      justify-content: center;
      padding-top:32px;
    }
}
@media(max-width:992px){
    .image-section{
        display:flex;
        align-items: center;
        justify-content: center;
        padding-top:36px;
       
    }
}
img{
    width:845px;
}
@media (max-width:992px){
    img{
       width:400px;
       
      
       
    }
}
</style>