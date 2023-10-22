<script>
  import NavBar from '../components/partials/NavBar.vue';
  import {newsList} from '../data/store'

  export default {
    name: 'Header',
    components:{
      NavBar 
    },
    data(){
      return {
        newsList
      }
    }
  }
</script>

<template>
  <header>
    <!-- newsUpdate -->
    <div class="newsUpdate">
      <div class="containerHead container d-flex justify-content-between">
        <div class="d-flex align-items-center">
          <div class="profileButton">
            <span class="buttonUpdates">NEWS UPDATES</span>
            <img class="profileImage" src="/image/ProfiloImage.jpg" alt="profilo">
          </div>
          <span v-for="news in newsList"
          :key="news.id"> {{news.hour}}.{{ news.minutes }}: {{ news.news }} </span>
        </div>
  
        <div class="socialHeader d-flex align-items-center">
          <div class="iconeArrow">
            <i class="fa-solid fa-chevron-left"></i>
            <i class="fa-solid fa-chevron-right"></i>
          </div>
          <div class="iconeSocial">
            icone
          </div>
        </div>
      </div>
    </div>
    <!-- /newsUpdate -->
    
    <!-- bannersection -->
    <section class="banner container d-flex justify-content-between align-items-center ">
      <div class="containerBanner">
        <img id="logo" src="/public/image/anime-logo-300x89.webp" alt="logo-red">
      </div>
      
      <div >
        <img class="bannerImage" src="/public/image/header-banner-300x38.webp" alt="banner">
      </div>
    </section>
    <!-- /bannersection -->

    <NavBar/>

  </header>
</template>

<style lang="scss">
  @use '../scss/header.scss';
</style>