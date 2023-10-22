<script>
import {cardsList} from '../../data/store'

  export default{
    name: 'ItemSection',
    data(){
      return {
        cardsList
      }
    }
  }
</script>

<template>

  <section class="itemsection py-4 d-flex">
    <div 
      v-for="card in cardsList"
      :key="card.id"
      class="card pippo m-1">

        <img class="card-img-top" :src="`/public/image${card.src}`" :alt="card.src">
        <div class="cardHover">
          <div class="posts h-75 m-3 d-flex flex-column justify-content-center ">
            <h6 class="d-none text-uppercase ">{{card.btn}}</h6>
            <span class="d-none text-uppercase ">4 POSTS</span>
          </div>
        </div>
     
    </div>

  </section>

</template>

<style lang="scss" scoped>
@use '../../scss/partials/variables' as *;
  .pippo {
    position: relative;
    .cardHover{
      position: absolute;
      width: 100%;
      height: 100%;
      color: $lightColor;
      text-align: center;

      &:hover{
        background-color: $primaryColor;
        opacity: .7;
        
        .posts {
          border: 1px solid white;
          vertical-align: middle;
          h6, span{
            display: block !important;
          }
        }
      }
    }
  }

</style>