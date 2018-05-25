<template>
  <div id="app">
      <app-hero/>
      

      <main class="maincontent">
      <app-cards/>

      <app-passion/>
      
      <app-description/>
      
      <app-cards/>
      <app-features/>
      <app-maker/>
      </main>

      <app-footer/>
      <div class="overlay"></div>

  </div>
</template>

<script>
import Hero from './components/Hero.vue'
import Nav from './components/Nav.vue'
import Footer from './components/Footer.vue'
import Cards from './components/Cards.vue'
import Passion from './components/Passion.vue'
import Description from './components/Description.vue'
import Features from './components/Features.vue'
import Maker from './components/Maker.vue'



export default {
  name: 'app',
  data () {
    return {
      
    }
  },

  components:{
    appHero: Hero,
    appFooter: Footer,
    appCards: Cards,
    appPassion: Passion,
    appDescription: Description,
    appFeatures: Features,
    appMaker: Maker,
   
    


  }
}
</script>

<style lang="scss">
   
   @import url('https://fonts.googleapis.com/icon?family=Material+Icons');
   @import url( 'https://fonts.googleapis.com/css?family=Montserrat:300,400,700,900');
   @import 'libs/normalize/normalize';
   @import 'libs/scss/adjustment';
   
   html,body{
     margin: 0;
     padding: 0;
     background: #110320;
     font-family: 'Montserrat', sans-serif;
     overflow-x: hidden;
   }
   a{
     text-decoration: none;
   }
   ul{
     padding: 0;
     margin: 0;
     list-style: none;
   }
   h1{
     margin: 0;
     padding: 0;
   }
   
   button{
     position: absolute;
     background: transparent;
     
     margin-top: 179px;
     outline: none;
     cursor: pointer;
     transform: translateX(2015%);
     border: 25px solid transparent;	
     border-left: 25px solid #eee;
   }

 


   

   



</style>
