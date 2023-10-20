<script>
import {cardsList} from '../../data/store'

  export default{
    name: 'Card',
    data(){
      return {
        cardsList
      }
    }
  }
</script>

<template>
  <div 
  v-for="card in cardsList"
  :key="card.id"
  class="card m-1">
  <img class="card-img-top" :src="`/public/image${card.src}`" :alt="card.src">
  <div class="card-body text-center">
    <h6 class="card-title">{{card.title}}</h6>
    <p class="card-text">{{card.date}}</p>
  </div>
</div>






</template>

<style lang="scss">
  @use '../../scss/partials/card.scss';
</style>