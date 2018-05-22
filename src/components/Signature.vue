<template>
  <div class="signature">
    <span class="signature__author">blaz robar</span>
    <span class="signature__words">paint the power</span>
    <button class="signature__arrow">
        <i class="material-icons">keyboard_arrow_down</i>
    </button>
  </div>
</template>

<script>
export default {
 data (){
   return{
     
   }
 }
}
</script>

<style lang="scss" scoped>
 
 @import '../libs/scss/adjustment';


  .signature{
    writing-mode: vertical-lr;
    position: absolute;
    left:23px;
    margin-top: 300px;

    @include customize (1030px){
      left: 19px;
    }

    @include customize (590px) {
      display: none;
    }
    
    
    
  }

  .signature__author{
    color: #b5bbc4;
    font-size: 10px;
    font-weight: 400;
    text-transform: uppercase;
    padding-bottom: 13px;
    word-spacing: 3px;
    
  }

  .signature__words{
    font-size: 12px;
    font-weight: 400;
    color: #fff;
    text-transform: uppercase;
    word-spacing: 2px;

  }

  .signature__arrow{
    background: none;
    border: none;
    outline: none;
    color: #fff;
    cursor: pointer;
   
    position: absolute;
    padding: 340px 0 0 0; 
    left: -2px;

    @include customize (1030px){
      left: -4px;
      padding-top: 280px; 
    }
       
   
  }
</style>
