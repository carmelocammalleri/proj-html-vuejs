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

      <!-- Visione Grande dell'elemento selezionato su youtube -->
      <div class="bigView">
        <img src="/public/image/sddefault.webp" class="w-100" alt="">
      </div>

      <!-- Lista video da guardare -->
      <div class="sectionVideos">
        <div class="videosPlaylist d-flex align-items-center">
          <i class="fa-solid fa-play mx-3"></i>
          <!-- Playlist titolo -->
          <div class="text">
            <span>Video Playlist</span>
            <br>
            <span>Videos</span>
          </div>
        </div>

        <!-- video non selezionati -->
        <div class="small-view">
          <div 
          v-for="card in cardsList"
          :key="card.id"
          class="video d-flex">
            <img :src="`/public/image${card.src}`" class="h-100 d-block" alt="">
            <div class="videoTextTitle">Video Playlist-Official Trailer- AniTv</div>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>

<style lang="scss">
  @use '../../scss/partials/youtubeSection.scss';
</style>