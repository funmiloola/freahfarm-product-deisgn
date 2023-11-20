<template>
  <div class="review-section">
   <h1>What Our Clients Have To Say</h1>
   <div class="reviews">
    <div v-for="(review,index) in reviews" :key="index" class="review">
        <div class="clients-details">
        <img :src="review.image" alt="">
        <h2>{{review.name}}<br><span>{{review.profession}}</span></h2>
        </div>
        <p>{{review.desc}}</p>
    </div>
   </div>
   <div class="subscription">
    <h3>Subscribe to Our Newsletter</h3>
    <p>Enter your Email Address below to get daily offers and news</p>
    <div class="sub-requirements">
    <input type="email" placeholder="Enter your Email">
    <button>Join Our Mail List</button>
    </div>
   </div>
  </div>
</template>

<script>
 
export default {
  data(){
    return{
        reviews:[
            {image:require('@/assets/images/Ellipse 1.svg'),name:'Reykiya Ahmad ',profession:'CEO Brandkit',desc:'Getting organic healthy meals has been a chore for me until I started using FreshFarm. My meals are delivered on time and I don’t have to stress or worry. I totally recommend them.'},
            {image:require('@/assets/images/Vector.svg'),name:'Hope Raymonds', profession:'CEO GrowthBank', desc:'Getting organic healthy meals has been a chore for me until I started using FreshFarm. My meals are delivered on time and I don’t have to stress or worry. I totally recommend them.'}
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
.review-section{
    max-width:1280px;
    margin:0 auto;
    border:1px solid red;
}
/* @media (max-width:992px){
    .review-section{
        max-width:900px;
    }
} */
 h1{
    text-align:center;
    padding-top:120px;
    font-family: inter;
    font-weight:700;
    font-size:40px;
 }
 @media (max-width:992px){
    h1{
        font-size:36px;
        padding-top:80px;
    }
 }
 .reviews{
      display:flex;
      padding-top:62px;
      justify-content: center;
      gap:20px;
 }
 @media (max-width:992px){
    .reviews{
        flex-direction:column;
        gap:36px;
        align-items: center;
        padding-top:56px;
    }
 }
 .review{
    border:1px solid hsla(0, 0%, 23%, 0.2);
    border-radius: 8px;
 }
 @media (max-width:992px){
    .review{
        width:300px;
    }
 }
 .clients-details{
    display:flex;
    align-items: center;
    gap:20px;
    padding-top:30px;
    padding-left:30px;
 }
@media(max-width:992px){
    .clients-details{
        flex-direction: column;
        align-items: flex-start;
        padding-top:16px;
        gap:16px;
    }
}
 h2{
    font-family: inter;
    font-size:20px;
    font-weight: 700;
 }
 @media(max-width:992px){
    h2{
        font-size:16px;
    }
 }
 span{
    color: #3a3a3a;
    font-family: inter;
    font-size:14px;
    font-weight:500;
 }
 .reviews p {
     /* width:527px; */
     color:#3a3a3a;
     font-size:14px;
     line-height:32.4px;
     font-family: inter;
     font-weight: 500;
     padding-top:20px;
     padding-left:30px;
     padding-right:33px;
     padding-bottom:30px;
 }
 @media (max-width:992px){
    .reviews p {
        width:250px;
        padding-right:0;
        padding-bottom:15px;
        padding-top:15px;
    }
 }
 h3{
    font-family:inter;
    font-size:40px;
    font-weight: 700;
    text-align: center;
    padding-top:120px;
 }
 @media (max-width:992px){
    h3{
        padding-top:80px;
        font-size:36px;
    }
 }
 .subscription p {
    padding-top:32px;
    text-align:center;
    color:#3a3a3a;
    font-family: inter;
    font-size:20px;
    font-weight: 500;
 }
 @media (max-width:992px){
    .subscription p {
        padding-top:28px;
        font-size:16px;
    }
 }
 .sub-requirements{
    display:flex;
    justify-content: center;
    gap:23px;
    padding-top:32px;
 }
 @media (max-width:992px){
    .sub-requirements{
        flex-direction: column;
        gap:36px;
    }
 }
 input{
    padding-top:15px;
    padding-bottom:14px;
    padding-left:30px;
    padding-right:222px;
    border:1px solid hsla(0, 0%, 23%, 0.2);
    border-radius: 8px;
    outline: none;
 }
 @media(max-width:992px){
   input{
      padding-right:100px;
      margin-left:10px;
      margin-right:10px;
   }
 }
 input::placeholder{
    font-size:20px;
    font-weight:500;
    font-family: inter; 
 }
 @media (max-width:992px){
    input::placeholder{
        font-size:16px;
    }
 }
 button{
    color:#fff;
    padding:20px 45px;
    background: #008000;
    border:none;
    border-radius:8px;
    font-family: inter;
    font-weight: 700;
    font-size:18px;
 }
 @media (max-width:992px){
    button{
        font-size: 16px;
        margin-left:10px;
        margin-right:10px;
    }
 }
 @media (max-width:992px){
    img{
        width:100px;
    }
 }
</style>