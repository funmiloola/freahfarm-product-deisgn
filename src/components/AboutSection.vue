<template>
  <div class="about">
   <div class="about-section">
    <div class="about-details">
        <h1>About Us</h1>
        <p>Organic food is grown without the use of synthetic chemicals, such as human-made pesticides and fertilizers, and does not contain genetically modified organisms (GMOs). Organic foods induce fresh produce, meats and dairy products as well as processed foods such as crackers, drinks, and frozen meals.</p>
        <button>Learn More</button>
    </div>
     <div class="about-images">
    <div class="image-section">
    <img src="@/assets/Rectangle 6.svg" id="first-image">
    <img src="@/assets/images/Rectangle 8.svg" id="second-image">
    </div>
    <div class="image">
        <img src="@/assets/images/Rectangle 7.svg" id="third-image">
    </div>
     </div>
   </div>
  </div>
</template>

<script>

export default {
  
}
</script>

<style scoped>
*{
    margin:0;
    padding:0;
}
.about{
   max-width: 1280px;
   margin:0 auto;
   padding-top:120px;
   border:1px solid red;
}
@media (max-width:992px){
    .about{
        padding-top:80px;
        padding-left:12px;
        padding-right:12px;
    }
}
 .about-section{
    display:flex;
    align-items:center;
    gap:58px;
 }
 @media (max-width:992px){
    .about-section{
       flex-direction: column;
       align-items: center;
       justify-content: center;
       gap:36px;
    }
 }
 @media (max-width:992px){
    .about-details{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
 }
.about-images{
    display:flex;
    align-items: center;
    gap:21px;
}
@media(max-width:992px){
   .about-images{
    align-items: center;
    justify-content: center;
    padding-top:56px;
   }
}
.image-section{
    display: flex;
    flex-direction: column;
    gap:30px;
}
h1{
    
    font-weight: 700;
    font-size:40px;
    font-family: inter;
}
@media (max-width:992px){
    h1{
        font-size:36px;
        text-align: center;
    }
}
p{
    font-family: inter;
    font-weight: 500;
    font-size:20px;
    padding-top:32px;
    color: #3a3a3a;
    line-height:32.4px;
}
@media (max-width:992px){
    p{
        font-size:16px;
        text-align: center;
    }
}
button{
    padding: 20px 45px 20px 45px;
    border:none;
    border-radius:8px;
    background: #008000;
    color:#fff;
    font-family:inter;
    font-weight: 700;
    font-size:18px;
    margin-top:32px;
}
@media(max-width:992px){
   #first-image{
           width:130px;
     }
}
@media(max-width:992px){
   #second-image{
           width:130px;
     }
}
@media(max-width:992px){
   #third-image{
           width:170px;
     }
}
</style>