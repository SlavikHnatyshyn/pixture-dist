<template>

    
    <!-- passion -->
  <section class="passion" id="passion">

  
  <!-- passion__content -->
  <div class="passion__content container">
  
 
  <span class="passion__title"></span>
  

    <!-- passion__descr--wrapp-->
  <div class="passion__descr--wrapp">

   <div class="passion__descr">
   
   <h3 class="passion__descr--title">
    Texture makes art
   </h3>
   <p class="passion__descr--text">
     Lorem ipsum dolor sit amet, 
     consectetur adipisicing elit, sed
     do eiusmod tempor incididunt ut labore et dolore magna aliqua.  
   </p>
   
   </div> <!-- ./passion__descr-->

   <span class="passion__time">April 19th 2016</span>
  


  </div>  <!-- ./passion__descr--wrapp-->
  
  
  


  </div> <!-- ./passion__content -->

   <app-signature/>
  
  </section> <!-- ./passion -->

</template>

<script>
import Signature from './Signature.vue' 


export default {
    data () {
      return{

      }
    },
     
    components:{
       appSignature: Signature,
    }  


}
</script>

<style  lang="scss" scoped>
  
  @import '../libs/scss/adjustment';
  
  .passion{
    height: 100vh;
    
<<<<<<< HEAD
    background: url('../assets/only.png') center center no-repeat;
=======
    background: url(../assets/3-1.png) center center no-repeat;
>>>>>>> master
    background-size: cover;
    padding: 20px 0  55px 0;

    @include small {
      padding-top: 0;
    }

    @include extraSmall {
      padding-bottom: 0;
           
    }

   

   
  }


  .passion__descr--wrapp{
    display: flex;
    justify-content: space-between;
    
    @include customize (1030px){
      justify-content: center;
      align-items: center;
    }

    
    
  }


  .passion__descr{
   padding: 280px 0 0 76px;
   transform: translateY(81%);
    
   @include customize (1030px){
    
    margin-top: 150px;
    text-align: center;
    transform: translateY(0);
     
   } 

   @include small {
    padding-left: 10px;
   }

  }

  .passion__descr--title{
    font-weight: 700;
    font-size: 24px;
    color: #fff;
    padding-bottom: 18px;
    
    margin: 0;
    
     @include customize (1030px){
      padding-bottom: 10px; 

     }

   


  }

  .passion__descr--text{
    width: 478px;
    font-size: 13px;
    font-weight: 400;
    color: #fff;
    padding: 0;
    margin: 0;
    line-height: 25px;

    @include customize (505px) {
      width: 300px;
    }
   
  }

  .passion__time{
    font-size: 13px;
    font-weight: 400;
    color: #fff;
    padding: 0;
    margin: 0;
    padding-top: 330px;
    transform: translateY(81%);

    @include customize (1030px){
      display: none;
    }
  }




</style>
