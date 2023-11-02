<template>
  <div>
   <section class="food-category">
    <div>
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
.food-category{
    display: flex;
    align-items:center;
    padding-left:22px;
}
.food-details{
    padding-left:103px;
}
h1{
    width:342px;
    height:104px;
    font-family:inter;
    font-weight:700;
    font-size:40px;
}
p{
    font-weight:500;
    font-size:20px;
    font-family:inter;
    line-height:32.4px;
    width:442px;
}
button{
     padding: 20px 75px 20px 75px;
    border:none;
    border-radius:8px;
    background: #008000;
    color:#fff;
    font-family:inter;
    font-weight: 700;
    font-size:18px;
    margin-top:32px;
}
</style>