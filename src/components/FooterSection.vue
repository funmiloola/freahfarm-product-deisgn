<template>
  <div class="footer">
   <div class="options">
    <ul>
      <li v-for="(detail,index) in details" :key="index">{{ detail }}</li>
    </ul>
    <div class="logo">
      <img :src="icon" alt="" v-for="(icon,index) in icons" :key="index">
      </div>
    </div>
    <footer>
      <div>
        <p><img src="@/assets/images/Vector (1).svg" alt="">2022 FreshFarm</p>
      </div>
      <ul>
        <li v-for="(policy,index) in policies" :key="index">{{policy}}</li>
      </ul>
    </footer>
  </div>
</template>

<script>
 
export default {
  data(){
    return{
      details:['Home','Menu','About Us','Contact Us'],
      icons:[require('@/assets/images/Linkedin.svg'),require('@/assets/images/Facebook.svg'),require('@/assets/Twitter.svg'),require('@/assets/images/Instagram.svg')],
      policies:['Privacy Policy','Terms & Conditions','Cookies Policy']
    }
  }
}
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Commissioner:wght@400;500;700&family=DM+Sans:opsz,wght@9..40,400;9..40,500&family=Inter:wght@400;500;700&family=Josefin+Sans:wght@400;700&family=Karla:wght@400;700&family=Kumbh+Sans:wght@400;700&family=League+Spartan:wght@500;700&family=Lexend+Deca&family=Manrope:wght@800&family=Pacifico&family=Plus+Jakarta+Sans:wght@500;800&family=Roboto:wght@400;700&family=Rubik:wght@400;500;700&display=swap');
*{
  margin:0;
  padding:0;
}
.footer{
  border:1px solid #f5f5f5;
  width:100%;
  max-width: 1440px;
  height: 285.218px;
  background: #f5f5f5;
  margin:120px 0px 0px 0px;
}
@media (max-width:992px){
  .footer{
    max-width:992px;
    width:100%;
  }
}
 .options{
  display:flex;
  justify-content: space-between;
  align-items: center;
  padding-top:103.31px;
  padding-left:49px;
  padding-right:35px;
  padding-bottom:40px;
  margin-left:100px;
  margin-right:99px;
  border-bottom:1px solid #cdd0c8;
 }
 @media (max-width:992px){
  .options{
    flex-direction:column;
    justify-content: center;
    gap:24px;
    padding-top:50px;
    padding-left:0;
    padding-bottom:0;
    margin-left:0;
    margin-right: 0;
    padding-right:0;
    border-bottom:none;
  }
 }
 .options ul{
  display: flex;
  gap:32px;
  color: #008000;
  font-family: Rubik;
  font-size: 15px;
  font-weight: 500;
  cursor:pointer;
 }
 @media(max-width:992px){
  .options ul {
    font-size: 12px;
  }
 }
 ul li{
  list-style-type: none;
 }
 footer{
  display:flex;
  justify-content: space-between;
  align-items: center;
  padding-top:30px;
  padding-left:139px;
  padding-right:130px;
 }
 @media (max-width:992px){
  footer{
    flex-direction:column;
    gap:24px;
    padding-left:0;
    padding-right:0;
    padding-top:36px;
  }
 }
 footer ul{
    display: flex;
    gap:26px;
    color: var(--Off-white, rgba(17, 17, 17, 0.50));
    font-family: Rubik;
    font-size: 12px;
   font-weight: 400;
 }
 p{
  display: flex;
  align-items: center;
  gap:6px;
  color: var(--Off-white, rgba(17, 17, 17, 0.50));
  font-family: Inter;
  font-size: 16px;
  font-weight: 600;
 }
 .logo{
  display:flex;
  gap:20px;
  align-items: center;
 }
 @media (max-width:992px){
  .logo{
    gap:36px;
  }
 }
</style>