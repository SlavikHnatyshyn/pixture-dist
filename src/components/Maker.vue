<template>
  <div class="maker--wrapp ">
      <div class="maker__content container">
      
      <span class="maker__by">Textures by</span>
      <span class="maker__author">Jordan Hetzer</span>
      
      <p class="maker__descr">Lorem ipsum dolor sit amet, 
        consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore.
      </p>

      </div>

  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

 @import '../libs/scss/adjustment';

.maker--wrapp{
  background: url(../assets/2.png) center center no-repeat;
  background-size: cover;
  height: 617px;
  width: 100%;
}

.maker__content{
    display: flex;
    flex-flow: column wrap;
    text-align: left;
    transform: translateX(60%);
    padding-top: 200px;

    @include customize (1030px){
         transform: translateX(40%);
    }

    @include customize (630px) {
         transform: translateX(20%);
    }

    @include customize (376px){
        transform: translateX(7%);
    }
   
}


.maker__by{
font-size: 20px;
color: #fff;
font-weight: 700;
}

.maker__descr{
    width: 370px;
    font-size: 13px;
    line-height: 25px;
    font-weight: 400;
    color: #d6d6d6;

    @include extraSmall {
        width: 300px;
    }
   
}


.maker__author{
    font-size: 40px;
    color: #fff;
    font-weight: 700;
    margin: 0;
    padding-top: 6px; 
    
}

</style>
