<script>
import {cardsList} from '../../data/store';
import {Swiper, SwiperSlide} from 'swiper/vue';
import 'swiper/css/navigation';
import 'swiper/css';

// inserisci le freccette
import { Navigation, Mousewheel, Keyboard } from 'swiper/modules';

  export default{
    name: 'CardSlider',
    components:{
      Swiper,
      SwiperSlide
    },
    data(){
      return {
        cardsList
      }
    },
    setup() {
      return {
        modules: [Navigation, Mousewheel, Keyboard]
      };
    }
  }
</script>

<template>
  <section class="slider">
    <Swiper :slidesPerView="4"
      :spaceBetween="8"
      :navigation="true"
      :centeredSlides="false"
      :modules="modules"
      class="mySwiper">

      <SwiperSlide v-for="card in cardsList"
          :key="card.id">
          <div class="card m-1">
            <img class="card-img-top" :src="`/public/image${card.src}`" :alt="card.src">
            <span class="btnInfo">{{card.btn}}</span>
            <div class="card-body text-center">
              <h6 class="card-title">{{card.title}}</h6>
              <p class="card-text">{{card.date}}</p>
            </div>
          </div>
      </SwiperSlide>

    </Swiper>
    

  </section>

</template>

<style lang="scss">
  @use '../../scss/partials/card.scss';
</style>