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
        <img src="@/assets/images/Rectangle 7.svg">
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
    padding-top:132px;
    padding-left:121px;
}
 .about-section{
    display:flex;
    align-items:center;
    gap:58px;
 }
.about-images{
    display:flex;
    align-items: center;
    gap:21px;
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
p{
    font-family: inter;
    font-weight: 500;
    font-size:20px;
    padding-top:32px;
    color: #3a3a3a;
    line-height:32.4px;
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