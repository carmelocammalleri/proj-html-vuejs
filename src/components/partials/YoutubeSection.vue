<script>
  import {cardsList} from '../../data/store';

  export default{
    name: 'YoutubeSection',
    data(){
      return{
        cardsList
      }
    }
  }
</script>

<template>
  <section class="youtubeSection container">
    <div class="containerDisplay my-5 d-flex">
      <div class="grande">
        <img src="/public/image/sddefault.webp" class="w-100" alt="">
      </div>
      <div class="lista">
        <div class="videosPlaylist d-flex align-items-center">
          <i class="fa-solid fa-play mx-3"></i>
          <div class="text">
            <span>Video Playlist</span>
            <br>
            <span>Videos</span>
          </div>
          
        </div>
        <div class="scan">
          <div v-for="card in cardsList"
          :key="card.id">
            <img :src="`/public/image${card.src}`" class="h-100" alt="">
            <span>Video Playlist</span>
              <br>
            <span>Videos</span>
          </div>
      
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss">
  @use '../../scss/partials/youtubeSection.scss';
</style>