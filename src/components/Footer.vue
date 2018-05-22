<template>
  <div class="footer__wrapp container" id="contacts">
  <ul class="footer">
      <li class="footer__about">
         <h3 class="footer__title exception">About</h3>
         <p class="footer__about--descr">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit, 
            sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
            Ut enim ad minim veniam, quis nostrud 
         </p>
      </li>
      
      <li class="footer__history">
          <h3 class="footer__title">History</h3>
          
          <a href="#" class="footer__history--link">Resources</a>
          <a href="#" class="footer__history--link">Downloads & Updates</a>
          <a href="#" class="footer__history--link">Manuals</a>
          <a href="#" class="footer__history--link">Tech Specs</a>
          <a href="#" class="footer__history--link">System Status</a>
          <a href="#" class="footer__history--link">Accessibility</a>

      </li>
      
      <li class="footer__contact">
          <h3 class="footer__title">Contact</h3>
          
          <address class="footer__contact--addr">
              <span class="addr__item">Apple Store (Education Institutions)</span>
              <span class="addr__item">1300-551-927</span>
              <span class="addr__item">Apple Store (Small Business)</span>
              <span class="addr__item">1300-551-927</span>  
          </address>

      </li>
       
</ul>

   <span class="footer__descr ">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repudiandae aut, pariatur.
   </span>

  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

  @import '../libs/scss/adjustment';
  
  .footer__wrapp{
      padding-bottom: 135px;

    @include extraSmall {
        padding: 0;
    }
     
  }
  
  .footer{
      padding-top: 70px; 
      padding-bottom: 72px;
      display: flex;

       @include customize (770px) {
          justify-content: center;
          
      } 

      @include extraSmall {
          flex-flow: column;
          align-items: center;
      }
  }

  .footer__title{
      color: #0d4160;
      font-size: 13px;
      font-weight: 400;
      text-transform: uppercase;
      margin: 0;
      padding-bottom: 22px;
  }

  .footer__about{
      padding-right: 32px;
  }

  .footer__about--descr{
      width: 266px;
      line-height: 24px;
      color: #fff;
      font-weight: 400;
      font-size: 12px;
      margin: 0;
      padding:0;
  }

  .footer__history{
      display: flex;
      flex-flow: column wrap;
      padding-right: 40px;

      @include customize (770px) {
          padding-right: 0;
      }

      @include extraSmall {
          padding-top: 40px;
      }
  }

  .footer__history--link{
      color: #fff;
      font-size: 12px;
      font-weight: 400;
      padding-bottom: 22px; 
  }

   .footer__contact{
       @include customize (770px){
           display: none;
       }
   }


  .footer__contact--addr{
      display: flex;
      flex-flow: column wrap;
  }

  .addr__item{
      color: #fff;
      font-size: 12px;
      font-weight: 400;
      padding-bottom: 22px; 
      font-style: normal;
  }

  .exception{
      padding-bottom: 18px;
  } 
   
  .footer__descr{
      font-size: 12px;
      font-weight: 400;
      color: #5c5b61;

      @include customize (770px) {
          display: flex;
          justify-content: center;
      }

      @include customize (536px) {
          display: none;
      }
  }   

</style>
