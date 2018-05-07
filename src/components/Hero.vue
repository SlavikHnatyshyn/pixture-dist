<template>
    
    <!-- hero -->
  <section class="hero" id="home">

   <!-- header-->
   <header class="header">
   
   
   <app-nav />
   
   
   
   <app-form/>

  </header> <!-- ./header-->

  <!-- hero__content -->
  <div class="hero__content container">
  
 
  <span class="hero__title">
   <img src="../assets/your.png" alt="your" class="hero__title--img">
  </span>

  <div class="hero__title--wrapp">
  
  <span class="hero__title--2">Paint</span>
  <span class="hero__title--2">your</span>
  <span class="hero__title--2">pixture</span>
  
  </div>

    <!-- hero__descr--wrapp-->
  <div class="hero__descr--wrapp">

   <div class="hero__descr">
   
   <h3 class="hero__descr--title">
     Humble Beginings
   </h3>
   <p class="hero__descr--text">
     Lorem ipsum dolor sit amet, consectetur adipisicing 
     elit, sed do eiusmod tempor incididunt ut labore et dolore 
     magna aliqua. 
   </p>
   
   </div> <!-- ./hero__descr-->

   <h1 class="hero__time">April 19th 2016</h1>
  


  </div>  <!-- ./hero__descr--wrapp-->
  
  
  


  </div> <!-- ./hero__content -->

  <app-signature/>
  
  </section> <!-- ./hero -->

</template>

<script>

import Nav from './Nav.vue'
import Form from './Form.vue'
import Signature from './Signature.vue'

export default {
    data () {
      return{

      }
    },
    components:{
      appNav:Nav,
      appForm: Form,
      appSignature: Signature, 

    }

}
</script>

<style lang="scss" scoped>
  
  @import '../libs/scss/adjustment';
  
  .hero{
    height: 100vh;
    background: url(../assets/b3.png) center center no-repeat;
    background-size: cover;
    padding-bottom: 55px;

  @include customize (1030px){
    height: 800px;
  }

  @include small {
    padding-bottom: 0;
  }
   
  

  }

 

  .hero__title{
    text-align: center;
    background-size: cover; 
  }

  .header{
    display: flex;
    justify-content: space-between;
  }

  .hero__descr--wrapp{
    display: flex;
    justify-content: space-between;
    
    
  }

  .hero__title{
    display: flex;
    justify-content: center;
    align-items: center;
    transform: translateY(60%);
        

    @include customize (1031px){
      display: none;
    }
  }

  .hero__title--wrapp{
    width: 380px;
    
    margin-left: 117px; 
  }


  .hero__title--2{
    color: #fff;
    font-size: 132px;
    font-weight: 700;
    margin: 0;
    padding: 0;
    text-align: left;
    line-height: 0.8;
    text-transform: uppercase;
    margin-top: 30px;
    display: none;
    
   @include customize (1030px){
     display: block;
   }

   @include small{
     font-size: 100px;
   }

   @include customize (593px) {
     font-size: 80px;
   }
    
   @include extraSmall {
     font-size: 50px;
     
   }


  }

  .hero__descr{
  padding: 280px 0 0 76px; 
  
  @include customize (1030px){
    padding-top:100px; 
  }

  @include extraSmall {
    padding-left: 30px;
   

    
  } 
  
  }


  .hero__descr--title{
    font-weight: 700;
    font-size: 24px;
    color: #fff;
    padding-bottom: 18px;
   
    margin: 0;

    @include extraSmall {
      font-size: 18px;
    }

  }

  .hero__descr--text{
    width: 478px;
    font-size: 13px;
    font-weight: 400;
    color: #fff;
    padding: 0;
    margin: 0;
    line-height: 25px;
    
    @include extraSmall {
      width: 300px;
    }

  }

  .hero__time{
    font-size: 13px;
    font-weight: 400;
    color: #fff;
    padding: 0;
    margin: 0;
    padding-top: 330px;

    @include customize (1030px){
    display: none;
    }
  }


  


</style>
