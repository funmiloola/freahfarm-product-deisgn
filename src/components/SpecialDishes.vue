<template>
  <div>
<div class="dishes-category">
    <h1>Special Dishes For All</h1>
    <p class="first-paragraph">Made with premium & 100% Organic vegetables</p>
    <div class="about-dishes">
    <div v-for="(dish,index) in dishes" :key="index" class="dishes-details">
        <img :src="dish.image" alt="">
        <p class="dish-name">{{dish.name}}</p>
        <p class="dish-desc">{{dish.desc}}</p>
    </div>
    </div>
    <div class="btn">
        <button>View All</button>
    </div>
</div>
  </div>
</template>

<script>
 
export default {
  data(){
    return{
        dishes:[
            {image:require('@/assets/images/unsplash_mW0LIBBHNdE.svg'), name:'Green Salad', desc:'A salad combined with a delicious cut of bacon and mixed with tasty and fresh sesame oil'},
            {image:require('@/assets/images/unsplash_bBzjWthTqb8.svg'),name:'Beef Salad', desc:'A salad combined with a delicious cut of bacon and mixed with tasty and fresh sesame oil'},
            {image:require('@/assets/images/unsplash_kcA-c3f_3FE.svg'),name:'Nut Salad', desc:'A salad combined with a delicious cut of bacon and mixed with tasty and fresh sesame oil'}
        ]
    }
  }
}
</script>

<style scoped>
*{
    margin:0;
    padding:0;
}
 .dishes-category{
    max-width:1280px;
    margin:0 auto;
 }
 h1{
    font-size:40px;
    font-weight:700;
    text-align:center;
    padding-top:80px;
    font-family:inter;
 }
 @media (max-width:992px){
    h1{
        font-size:32px;
    }
 }
.first-paragraph{
     font-size:20px;
     font-weight:500;
     color: #3a3a3a;
     text-align:center;
     padding-top:32px;
 }
@media (max-width:992px){
    .first-paragraph{
        font-size:16px;
        padding-top:24px;
    }
}
 .about-dishes{
    display:flex;
    justify-content: center;
    padding-top:71px;
    gap:74px;
    padding-right:12px;
    padding-left:12px;
 }
 @media (max-width:1200px){
    .about-dishes{
        gap:24px;
    }
 }
 @media (max-width:992px){
    .about-dishes{
        flex-direction: column;
        align-items: center;
        gap:36px;
    }
 }
 .dishes-details{
    border:1px solid hsla(0,0%,23%,0.1);
    border-radius: 8px;
    text-align: center;
    /* width:328px; */
    
 }
 @media (max-width:992px){
    .dishes-details{
        width:270px;

    }
 }
 .dishes-details img{
    padding-top:39px;
    width:250px;
 }
  @media (max-width:992px){
    .dishes-details img{
        width:200px;
    }
}
.dish-name{
    padding-top:18px;
    font-size:20px;
    font-weight:700;
    font-family:inter;
}
@media (max-width:992px){
    .dish-name{
        font-size:16px;
    }
}
.dish-desc{
    padding:18px 40.5px;
    width:227px;
    font-size:14px;
    line-height: 32.4px;
    font-family:inter;
}
@media (max-width:992px){
    .dish-desc{
        padding:18px 24px;
    }
}
.btn{
    display:flex;
    align-items:center;
    justify-content: center;
    padding-top:50px;
}
button{
    padding:20px 45px;
    background: #008000;
    border:none;
    border-radius:8px;
    font-size:18px;
    font-family: inter;
    font-weight:700;
    color:#fff;
}

</style>
