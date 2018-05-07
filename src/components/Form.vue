<template>
  <div class="wrapp">
  
  <button class="email-btn" @click="onEmailClick">
    <i class="material-icons">email</i>
  </button>

 

  <div class="form__wrapp" v-if="invalid">
 <button class="form__close-btn" @click="onCloseClick">
    <i class="material-icons">clear</i>
  </button>
  

  
  <form  class="form">
    <textarea cols="30" rows="5" class="form__textarea" maxlength="300" placeholder="Enter your message">

    </textarea>
    <button class="form__button" @click.prevent="onSubmitClick" >Submit</button>
  </form>
  

  </div> <!-- ./form__wrapp -->
  
  
  </div> 
</template>

<script>

import Modal from './Modal.vue'

export default {
  
  data: () =>({
    invalid: false,
    

  }),

  methods:{
    onEmailClick () {
      this.invalid = true;
    },

    onCloseClick () {
     this.invalid = false;
    },

    onSubmitClick () {
     let getValue = document.querySelector('.form__textarea').value;
     localStorage.setItem('formKey', getValue);
 
     setTimeout(this.invalid = false,3000);
    
    },
    
    

  },

  components: {
  appModal: Modal 
  },

 
 
}
</script>

<style lang="scss" scoped>

@import '../libs/scss/adjustment';
  

.email-btn{
    padding: 45px 50px 0 0;
    background: none;
    border: none;
    outline: none;
    color: #fff;
    margin: 0;
    cursor: pointer;
    
   @include customize (775px){
     display: none;
   }
}

.form__wrapp{
  background: #000;
  opacity: .9; 
  width: 100%;
  height: 100%;
  /*position: absolute;*/
  display: flex;
  justify-content: center;
  align-items: center;
  right: 0;
  top: 0; 
  z-index: 999;
  position: fixed;
}

.form{
 display: flex;
 flex-direction: column;
 align-items: center;
 z-index: 999;
 text-align: center;
 position: fixed;
}

.form__textarea{
  width: 400px;
  height: 200px;
  resize: none;
  outline: none;
  
}

.form__button{
  outline: none;
  border:none;
  padding: 10px;
  margin-top: 10px;
  width: 407px;
  cursor: pointer;
  color: #fff;
  background: #530649;
}

.form__close-btn{
  z-index: 9999; 
  position: fixed;
  cursor: pointer;
  background: #530649;
  border: none;
  color: #fff;
  outline: none;
  transform: translateY(-520%);
  right: 30px;
}

.form__close-btn > i {
   font-size: 50px;
   
}



</style>
