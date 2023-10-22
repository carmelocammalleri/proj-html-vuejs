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
          <!-- <span v-for="news in newsList"
          :key="news.id"> {{news.hour}}.{{ news.minutes }}: {{ news.news }} </span> -->
        </div>
  
        <div class="socialHeader d-flex align-items-center">
          <div class="iconeArrow mx-5">
            <i class="fa-solid fa-chevron-left mx-3"></i>
            <i class="fa-solid fa-chevron-right"></i>
          </div>
          <div class="iconeSocial">

              <i class="fa-brands fa-facebook m-1 p-1 bord"></i>

              <i class="fa-brands fa-twitter m-1 p-1 bord"></i>

              <i class="fa-brands fa-instagram m-1 p-1 bord"></i>

              <i class="fa-brands fa-youtube m-1 p-1 bord"></i> 

            
          </div>
        </div>
      </div>
    </div>
    <!-- /newsUpdate -->
    
    <!-- bannersection -->
    <section class="banner container d-flex justify-content-between align-items-center ">
      <div class="containerBanner d-flex justify-content-between align-items-center ">
        <div>
          <img id="logo" src="/public/image/anime-logo-300x89.webp" alt="logo-red">
        </div>
        <div class="bannerImage">
          <img src="/public/image/header-banner.webp" alt="banner">        
        </div>
        
      </div>
    </section>
    <!-- /bannersection -->

    <NavBar/>

  </header>
</template>

<style lang="scss">
  @use '../scss/header.scss';
</style>