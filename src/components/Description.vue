<template>
  
  <div>
  
  <div class="descr--wrapp container" id="articles">

   
    <p class="descr__1">
        Lorem ipsum dolor sit amet, consectetur adipisicing 
        elit, sed do eiusmod tempor incididunt ut labore et dolore
         magna aliqua. Ut enim ad minim veniam, quis nostrud 
         exercitation ullamco laboris nisi ut aliquip ex ea 
         commodo consequat. Duis aute irure dolor in reprehenderit 
         in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
         Excepteur sint occaecat cupidatat non proident, 
        sunt in culpa qui officia deserunt mollit anim id est laborum. 
    </p>

    <p class="descr__2">
        Sed ut perspiciatis unde omnis iste natus error sit
        voluptatem accusantium doloremque laudantium, totam 
        rem aperiam, eaque ipsa quae ab illo inventore 
        veritatis et quasi architecto beatae vitae dicta sunt explicabo. 
    </p>
   
   

   <p class="descr__3">
       Lorem ipsum dolor sit amet, consectetur adipisicing 
       elit, sed do eiusmod tempor incididunt ut labore et
       dolore magna aliqua. Ut enim ad minim veniam, quis
       nostrud exercitation ullamco laboris nisi ut aliquip 
       ex ea commodo consequat. Duis aute irure dolor in
       reprehenderit in voluptate velit esse cillum dolore 
       eu fugiat nulla pariatur. Excepteur sint occaecat
       cupidatat non proident, 
       sunt in culpa qui officia deserunt mollit anim id est laborum. 
   </p>


  </div> <!-- ./descr--wrapp -->
   
   <span class="descr__date"> 2016 january  </span>



  </div>

</template>

<script>



export default {
  
 

}
</script>

<style lang="scss" scoped>
  
  @import '../libs/scss/adjustment';

  .descr--wrapp{
      
      display: flex;
      flex-flow: row wrap;
      padding: 50px 0 0 161px;
      
      margin:0 
      -webkit-linear-gradient(left,  #1e0624 21%,#110320 39%,#1e0624 82%); /* Chrome10-25,Safari5.1-6 */
      
      @include customize (1030px) {
          padding-left: 0;
          padding-bottom: 50px;
          justify-content: center;

      }

      @include customize (590px) {
          padding: 20px;
      }
      
      @include extraSmall {
          
          
      }

}


  .descr__1{
     
      color: #d6d6d6;
      font-size: 13px;
      line-height: 25px;
      font-weight: 400;
      width: 517px;
      padding-right: 25px;
     
     width: 517px;
        @include customize (580px) {
          font-size: 12px;
          padding-right: 0;
          display: flex; 
          flex-flow: row wrap;
          justify-content: center;
          

      }

      @include customize (590px){
          padding-right:0; 
      }
  }
  
  .descr__2{
      
      color: #d6d6d6;
      font-size: 13px;
      line-height: 25px;
      font-weight: 400;
      width: 517px;
      padding-right: 25px;
      
      width: 517px;
        @include customize (580px) {
          font-size: 12px;
          padding-right: 0;
          display: flex; 
          flex-flow: row wrap;
          justify-content: center;
          

      }

      @include customize (590px){
          padding-right:0; 
      }
  }
  .descr__3{
      color: #d6d6d6;
      font-size: 13px;
      line-height: 25px;
      font-weight: 400;
      width: 517px;
      padding-right: 25px;

       @include customize (580px) {
          font-size: 12px;
          padding-right: 0; 
      }

      @include extraSmall {
          display: none;
      }
       
      @include customize (590px){
          padding-right:0; 
      }
  }

  .descr__date{
      text-transform: uppercase;
      color: #d6d6d6;
      font-size: 12px;
      font-weight: 400;
      writing-mode: vertical-lr;
      transform: translateY(-220%);
      padding: 0 0 0 26px;

      @include customize (1030px){
          display: none;
      }
      
    
  }
</style>
