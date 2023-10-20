<script>
import {cardsList} from '../../data/store';
import {Swiper, SwiperSlide} from 'swiper/vue';
import 'swiper/css/navigation';
import 'swiper/css';

import { Navigation, Mousewheel, Keyboard } from 'swiper/modules';

  export default {
    name: 'FeaturedPosts',
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
  <section class="slider bg-white p-3">
    <div class="container">
        <h4>FEATURED POST</h4>
        <div class="cardSection">

            <Swiper :slidesPerView="3"
                  :spaceBetween="8"
                  :navigation="true"
                  :centeredSlides="false"
                  :modules="modules"
                  class="mySwiper">
          
                <SwiperSlide 
                       v-for="card in cardsList"
                      :key="card.id">

                  <div class="card">
                        <img class="card-img-top" :src="`/public/image${card.src}`" :alt="card.src">
                   <div class="card-body text-center">
                        <h6 class="card-title">{{card.title}}</h6>
                        <p class="card-text">{{card.date}}</p>
                        <p class="card-text">{{ card.description }}</p>
                    </div>
                  </div>

                </SwiperSlide>
            </Swiper>
        </div>
    </div>
  </section> 
</template>

<style lang="scss">

</style>
