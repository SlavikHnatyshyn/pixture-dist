<template>
  <div>
  
  <h3 class="cards__title">Pictures worth seeing</h3>
  
  
  
  
    
   <slick class="cards--wrapp" id="pictures"    ref="slick" :options="slickOptions">
     <!-- card -->
   <div class="card ">
    
    <div class="card__img">
      <span class="card__liks">&#x2764; 382</span>
    </div>
    
    

    <!-- card__content -->
    <div class="card__content">
     
     <h2 class="card__title">decayed</h2>
     <p class="card__descr">
      Lorem ipsum dolor sit amet, consectetur adipisicing 
      elit, sed do eiusmod tempor incididunt ut labore et dolore
       magna aliqua.
     </p>

     <div class="triangle"></div>

       <!-- ./card__comment--wrapp -->
     <div class="card__comment-wrapp">
       
        <!-- card__comment -->
       <div class="card__comment">

       <div class="card__comment--icon">
         <i class="material-icons">chat_bubble</i>
       </div>
       <span class="card__comment--descr">
         374 comments
       </span>

       </div>  <!-- ./card__comment -->

       <button class="card__comment--add">
         <i class="material-icons">more_horiz</i>
       </button>

     </div> <!-- ./card__comment--wrapp -->
    
    </div> <!-- ./card__content -->
   
   </div> <!-- ./card -->




  
   <div class="card">
    
    <div class="card__img">
      <span class="card__liks">&#x2764; 382</span>
    </div>
    
    <!-- card__content -->
    <div class="card__content">
     
     <h2 class="card__title">decayed</h2>
     <p class="card__descr">
      Lorem ipsum dolor sit amet, consectetur adipisicing 
      elit, sed do eiusmod tempor incididunt ut labore et dolore
       magna aliqua.
     </p>

     <div class="triangle"></div>

       <!-- ./card__comment--wrapp -->
     <div class="card__comment-wrapp">
       
        <!-- card__comment -->
       <div class="card__comment">

       <div class="card__comment--icon">
         <i class="material-icons">chat_bubble</i>
       </div>
       <span class="card__comment--descr">
         374 comments
       </span>

       </div>  <!-- ./card__comment -->

       <button class="card__comment--add">
         <i class="material-icons">more_horiz</i>
       </button>

     </div> <!-- ./card__comment--wrapp -->
    
    </div> <!-- ./card__content -->
   
   </div> <!-- ./card -->


     <div class="card">
    
    <div class="card__img">
      <span class="card__liks">&#x2764; 382</span>
    </div>
    
    <!-- card__content -->
    <div class="card__content">
     
     <h2 class="card__title">decayed</h2>
     <p class="card__descr">
      Lorem ipsum dolor sit amet, consectetur adipisicing 
      elit, sed do eiusmod tempor incididunt ut labore et dolore
       magna aliqua.
     </p>

     <div class="triangle"></div>

       <!-- ./card__comment--wrapp -->
     <div class="card__comment-wrapp">
       
        <!-- card__comment -->
       <div class="card__comment">

       <div class="card__comment--icon">
         <i class="material-icons">chat_bubble</i>
       </div>
       <span class="card__comment--descr">
         374 comments
       </span>

       


       </div>  <!-- ./card__comment -->

       <button class="card__comment--add"
       @click="onAddCommentClick"
       >
         <i class="material-icons">more_horiz</i>
       </button>

      

     </div> <!-- ./card__comment--wrapp -->
    
    </div> <!-- ./card__content -->
   
   </div> <!-- ./card -->



    <button class="sliderBtn" >
     <i class="material-icons">keyboard_arrow_right</i>
   </button>

   </slick>  

  
  
  

  
  

  </div>
  
</template>



<script>



import Slick from 'vue-slick';
import AddComment from './AddComment.vue'


export default {
  
  
  data: () => ({
          show: false,
          slickOptions: {
            
           
            infinite: true,
            slidesToShow: 2,
            slidesToScroll: 1,
            variableWidth:true,
            
            
           
            
            
            prevArrow: 'none',
            
           
                
            },
      
  }),
  methods:{
    onAddCommentClick () {
      this.show = true
    },

     
  },

   components: { 
    Slick,
    appAddComment: AddComment,

   
   },


}



</script>

<style lang="scss" scoped>

@import  '../../node_modules/slick-carousel/slick/slick.scss';
@import '../libs/scss/adjustment';



.cards--wrapp{
  display: flex;
  
  
}


.cards__title{
    padding: 0 0 45px 76px;
    margin: 0;
    color: #f5f5f5;
    font-weight: 400;
    font-size: 18px;
    text-transform: uppercase;

    @include extraSmall {
      padding-bottom: 20px;
    }
}

.card{
  width: 381px !important;
  height: 468px;
  background: #fff;
  margin: 0 18px 21px 18px;
  
  outline: none;
  
}


.card__img{
  width: 381px;
  height: 205px;
  background: url(../assets/cardbg.png);
  background-size: cover;
  outline: none;
}

.card__liks{
  color: #fff;
  font-size: 12px;
  margin: 174px 0 0 321px;
  position: absolute;

}

.card__content{
  width: 264px;
}


.card__title{
  margin: 43px 0 25px 43px;
  color: #0c2539;
  font-weight: 700;
  font-size: 25px;
  line-height: 25px;
  text-transform: uppercase;
}

.card__descr{
  color: #677278;
  padding: 0;
  margin: 0 0 0 43px;
  width: 287px;
  font-weight: 400;
  font-size: 13px;
  line-height: 24px;
}

.triangle{
  border: 20px solid transparent;	border-left: 20px solid #110320;
  transform: translateY(-463%);
}

.card__comment-wrapp{
  height: 60px;
  width: 381px;
  background: #e9e9e9;
  display: flex;
  justify-content: space-between;
}

.card__comment{
  display: flex;
  padding: 23px 0 0 30px;
}

.card__comment--icon {
   color: #d5d5d5;
   padding-right: 10px;
}

.card__comment--descr{
  font-size: 14px;
  color: #0c2539;
  font-weight: 700;
  padding-top: 2px; 
}

.card__comment--add{
  color: #0b2235;
  background: ebebeb;
  border: none;
  outline: none;
  padding: 5px 24px 0 24px;
  cursor: pointer;
}

.card__comment--add > i{
  font-size: 30px;
}


.sliderBtn{
  background: #110320;
  border-radius: 50%;
  outline: none;
  border: none;
  cursor: pointer;
  height: 50px;
  width: 50px !important ;
  margin-top: 180px;
  position: absolute;
  right: 30px;

  @include small {
    display: none;
  }

}

.sliderBtn > i { 
  color: #fff;
  font-size: 60px;
  position: absolute;
  right: -6px;
  top: -3px;
}


</style>
