<script>
import {liveStyleElement} from '../../data/store'

  export default {
    name: 'lifeStyle',
    data(){
      return{
        liveStyleElement
      }
    },
    computed : {
    getArray (){
      return liveStyleElement.filter( element => element.id != '4' )
    }
  }
  }
</script>

<template>
  <section class="lifeStyle py-5">
    <div class="container">
      <h4>Lifestyles & stories</h4>
      
      <div class=" presentation d-flex">
        <div class="card presentationPhotos">
          <div class=" bg-black">

            <img class=" opacity-50" :src="`/public/image${liveStyleElement[3].src}`" alt="success">
          </div>
          <div class="d-inline-block position-relative">
                <div class="d-inline-block infoLifeStyle position-absolute bottom-50 text-white">
                  <i class="fa-solid fa-user m-1"></i><span>{{liveStyleElement[3].user}}</span>
                  <i class="fa-regular fa-calendar-days mx-1"></i><span>{{liveStyleElement[3].date}}</span> <br>
                  <span>{{liveStyleElement[3].title}}</span>
                </div>
              </div>
        </div>

        <div class="listPhotos">
          <div
            v-for="element in getArray"
            :key="element.id"
            class="foto">
            <div 
              class="imgCard d-flex align-items-center">
              <div class="imageBtnPosition">
                <img :src="`/public/image${element.src}`" alt="travel">
                <span class="btnPosition">{{element.btn}}</span>
              </div>

              <div class="d-inline-block">
                <div class="d-inline-block infoLifeStyle">
                  <i class="fa-solid fa-user m-1"></i><span>{{element.user}}</span>
                  <i class="fa-regular fa-calendar-days mx-1"></i><span>{{element.date}}</span> <br>
                  <span>{{element.title}}</span>
                </div>
              </div>

            </div>
          </div>

        </div>
      </div>

    </div>
  </section>
</template>

<style lang="scss">
  @use '../../scss/partials/lifeStyle.scss';
</style>