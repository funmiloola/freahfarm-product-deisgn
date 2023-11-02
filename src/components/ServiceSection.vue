<template>
  <div>
   <div class="header">
    <h1>Why Choose Us</h1>
    <p>Want to know why we stand out from the rest? Here's why!</p>
   </div>
   
 <div class="services">
    <div v-for="service in services" :key="service.index" class="contents">
    <img :src="service.image">
    <p class="title">{{service.title}}</p>
    <p class="content">{{service.content}}</p>
    </div>
   </div>
   <div class="details">
   <div v-for="detail in details" :key="detail.index" class="detail-contents">
    <h3>{{detail.total}}</h3>
    <p>{{detail.title}}</p>
   </div>
   </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
    services:[
        {image:require('@/assets/images/image 1.svg'), title:'Easy To Order', content:'Our Meals are easy to order and readily available'},
        {image:require('@/assets/images/image 4.svg'), title:'Worldwide Delivery', content:'We deliver to everywhere in the world for a fee'},
        {image:require('@/assets/images/image 6.svg'), title:'100% Organic', content:'Organic meals are grown without use of chemicals'}
    ],
    details:[
        {total:'400+', title:'Food Partners'},
        {total:'500+', title:'Trusted Clients'},
        {total:'10k+', title:'Orders Online'}
    ]
    }
  }
}
</script>
<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Commissioner:wght@400;500;700&family=DM+Sans:opsz,wght@9..40,400;9..40,500&family=Inter&family=Josefin+Sans:wght@400;700&family=Karla:wght@400;700&family=Kumbh+Sans:wght@400;700&family=League+Spartan:wght@500;700&family=Lexend+Deca&family=Manrope:wght@800&family=Pacifico&family=Plus+Jakarta+Sans:wght@500;800&family=Roboto:wght@400;700&display=swap');
*{
    padding:0;
    margin:0;
}
h1{
   
    font-family:inter;
    font-size:40px;
    font-weight:700;
    color:#000;
    padding-left:565px;
}
.header p{
   font-family:inter;
   font-size:20px;
   font-weight:500;
   color: #3a3a3a;
   padding-top:32px;
   padding-left:440px;
}
.services{
    display:flex;
    gap:74px;
    padding-top:62px;
    padding-left:187px;
}

.contents{
    display:flex;
    flex-direction: column;
    align-items: center;
    gap:15px;
    border:1px solid hsla(0, 0%, 23%, 0.1);
    border-radius:8px;
    padding-top:23px;
    width:303px;
    height:277px;
}
.title{
    font-family:inter;
    font-size:20px;
    font-weight: 700;
    color:#000;
}
.content{
    width: 192px;
    height:98px;
    font-family: inter;
    font-weight: 500;
    font-size:20px;
    text-align: center;
    line-height:32.4px;
    color:#3A3A3A;
}
.details{
     display:flex;
     padding-left:441px;
     padding-top:57px;
     gap:72px; 
}
.detail-contents{
    display:flex;
    flex-direction: column;
    gap:15px;
    align-items: center;
}
h3{
    font-weight:700;
    font-size:32px;
}
.detail-contents p {
    font-weight: 500;
    font-size:20px;
    color:#3A3A3A;
}
</style>
