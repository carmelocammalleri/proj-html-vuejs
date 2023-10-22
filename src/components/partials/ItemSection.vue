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
     
    </div>

  </section>

</template>

<style lang="scss" scoped>


</style>