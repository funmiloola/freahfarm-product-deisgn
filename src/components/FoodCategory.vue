<template>
  <div class="food-section">
   <section class="food-category">
    <div class="image">
       <img src="@/assets/images/unsplash_NDyuR4Huig8.svg" >
    </div>
    <div class="food-details">
        <h1>Fresh Vegetables Every Day</h1>
        <p>Healthy life can not be overemphasized. Our vegetables are organically grown without no added chemicals so users would live a healthy life.</p>
        <button>Learn More</button>
    </div>
   </section>
  </div>
</template>

<script>
 
export default {
  
  
}
</script>
<style scoped>
.food-section{
    padding-right:16px;
    padding-left:16px;
     max-width: 1280px;
    margin:0 auto;
}
.food-category{
    display: flex;
    align-items:center;
    justify-content: space-between;
   
}
@media (max-width:992px){
    .food-category{
        flex-direction: column;
        align-items:center;
        justify-content: center;
        padding-left:12px;
        padding-right:12px;
    }
}
h1{
    /* padding-right:72px; */
    font-family:inter;
    font-weight:700;
    font-size:40px;
    
}
@media (max-width:992px){
    h1{
        font-size:36px;
        text-align: center;
        padding-right:0;
        /* width:100%; */
    }
}
p{
    /* padding-right:54px; */
    font-weight:500;
    font-size:20px;
    font-family:inter;
    line-height:32.4px;
    color:#3a3a3a;
    /* width:422px; */
}
@media (max-width:992px){
    p{
        font-size:16px;
        text-align:center;
        padding-right:0;
        /* width:100%; */
    }
}
image{
    width:50%;
}
.food-details{
    width:50%;
}
@media (max-width:992px){
    image{
        width:100%;
    }
}
@media (max-width:992px){
    .food-details{
        width:100%;
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
img{
    width:600px;
}
@media (max-width:992px){
    img{
        width:375px;
        min-width:253px;
        display: block;
        margin:0 auto;
        padding-top:28px;
    }
}
@media (max-width:992px){
    .food-details{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
}
</style>