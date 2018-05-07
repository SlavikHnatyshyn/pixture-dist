<template>
  <div >
  
  <div class="cards--wrapp"  v-for="(card, key) in cards " :key="key" >
    <app-cards: cards="card" />
  </div>
  
  </div>
   
  


</template>

<script>

import Cards from './Cards.vue'

export default {
 
  data: () => ({
       cards: [
        { title: 'decayed', descr: ' Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et doloremagna aliqua.', cardsComment: ' 374 comments', id: 1 },
        { title: 'Bliss Texture', descr: ' Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et doloremagna aliqua.', cardsComment: ' 374 comments', id: 2 },
        
      ]
  }),

  components:{
      appCards: Cards,
  }


}
</script>

<style lang="scss" scoped>
 
 .cards--wrapp{
  display: flex;
}

</style>
