<template>
  <div class="features__wrapp">
      <ul class="features__list container" id="features">
          <li class="features__item">
              <h3 class="features__title">Start-Up Resources</h3>
              <p class="features__descr">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, 
                  sed do eiusmod tempor incididunt 
                  ut labore et dolore magna aliqua. Ut enim ad minim 
                  veniam, quis 
              </p>
          </li>
          <li class="features__item">
              <h3 class="features__title">Training & Funding</h3>
              <p class="features__descr">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, 
                  sed do eiusmod tempor incididunt 
                  ut labore et dolore magna aliqua. Ut enim ad minim 
                  veniam, quis 
              </p>
          </li>
          <li class="features__item">
              <h3 class="features__title">Connect</h3>
              <p class="features__descr">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, 
                  sed do eiusmod tempor incididunt 
                  ut labore et dolore magna aliqua. Ut enim ad minim 
                  veniam, quis 
              </p>
          </li>
          <li class="features__item">
              <h3 class="features__title">Communicate</h3>
              <p class="features__descr">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, 
                  sed do eiusmod tempor incididunt 
                  ut labore et dolore magna aliqua. Ut enim ad minim 
                  veniam, quis 
              </p>
          </li>
      </ul>

      <span class="features__date"> <span class="features__date--th">24th</span>2016 january </span>


  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>


@import '../libs/scss/adjustment';

.features__wrapp{
    margin: 0;
    padding: 0;
}



.features__list{
    padding:0 0 0 150px;
    display: flex;
    background: rgb(17,3,32);
    background: linear-gradient(90deg, rgba(17,3,32,1) 17%, rgba(21,1,36,1) 31%, rgba(17,3,32,1) 48%, rgba(21,1,37,1) 64%, rgba(17,3,32,1) 75%);
    flex-flow: row wrap;
    
    
    @include small{
        padding-left:0;
        padding-top: 50px; 
        align-items: center;
        justify-content: center; 
      
    }

    @include customize (590px) {
        padding-top: 0;
    }


    
}

.features__item{
    &:not(:last-child){
        padding-right: 27px; 
    }

    padding-bottom: 50px;

    @include customize (579px) {
        &:last-child{
            display: none;
        }
    }
}

.features__title{
    color: #fff;
    font-weight: 600;
    font-size: 25px;
    margin: 0;
    padding: 0 0 27px 0;

}

.features__descr{
    color: #d6d6d6;
    font-size: 13px;
    line-height: 25px;
    font-weight: 400;
    width: 268px;
    margin: 0;
    
}

.features__date{
    text-transform: uppercase;
    color: #d6d6d6;
    font-size: 12px;
    font-weight: 400;
    writing-mode: vertical-lr;
    padding-left: 26px; 
    word-spacing: 1px;
    transform: translateY(-165%);

    @include small {
        display: none;
    }
    
}

.features__date--th{
    
    color: #112037;

}







</style>
