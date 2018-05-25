<template>
   
   
  <nav class="nav">
  
  <button class="menu-btn" @click="onNavClick"
  :class="{ 'menu-btn--active' : invalid }"
  >
    <i class="material-icons">dehaze</i>
  </button>

   <div class="overlay"
   
   v-if="invalid"
   @click="onOverlayClick"
   ></div>


  <ul class="nav__list"
  v-if="invalid"
  
  >
 

    
  

    <li class="nav__item">
      <a href="#home" class="nav__link">Home</a>
    </li>
    <li class="nav__item">
      <a href="#pictures" class="nav__link">Pictures</a>
    </li>
    <li class="nav__item">
      <a href="#passion" class="nav__link">Passion</a>
    </li>
    <li class="nav__item">
      <a href="#articles" class="nav__link">Articles</a>
    </li>
    <li class="nav__item">
      <a href="#features" class="nav__link">Features</a>
    </li>
    <li class="nav__item">
      <a href="#contacts" class="nav__link">Contacts</a>
    </li>
  </ul>

  

  </nav>
  
  

  
  


</template>

<script>


(function($){
             
  $(function(){
     $('.nav a[href^="#"]').on('click', function (e) {
        e.preventDefault();

        let $anchor = $(this).attr('href');
        let $offsetTop = $($anchor).offset().top;

        $('body, html').animate({
            scrollTop: $offsetTop,
        }, 1000)
  })
  

    })(jQuery);

 })

export default {


  
  
  data(){
   return{
     invalid: false,
   }
  },
  
  methods:{
    onNavClick () {
    
    this.invalid = !this.invalid;
    },

    onOverlayClick () {
      this.invalid = false;
    }, 
  },
}

</script>

<style lang="scss" scoped>

@import '../libs/scss/adjustment';

.menu-btn{
    padding: 43px 0 0 22px !important;
    background: none;
    border: none;
    outline: none;
    color: #fff;
    cursor: pointer;
    transform: translateX(0);
    margin-top:0; 
   
    z-index: 999;
    
    @include customize (1030px){
      background: #140327;
      padding: 22px !important;
    }
    
}

.menu-btn--active{
  position: fixed;
}

.nav{
  display: flex;
  position: relative;
  z-index: 999;
  
}

.nav__list{
  
  background: #130325;
  flex-flow: column wrap; 
  position: fixed;
  top:0;
  padding:80px 80px 80px 0; 
  
 
}



.nav__item{

  padding: 20px 22px;
 
}

.nav__link{
  color: #fff;
}

.overlay{

   width: 100%;
   height: 100vh;
   background: #000;
   position: fixed;
   top:0;
   opacity: .9;
   
   }

 

   .body-fixed{
     width:100%;
     overflow: hidden;
   }








</style>
