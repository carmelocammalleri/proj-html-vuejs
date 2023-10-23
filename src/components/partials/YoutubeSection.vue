<script>
  import {videoInfo} from '../../data/store';


  export default{
    name: 'YoutubeSection',
    data(){
      return{
        videoInfo,
        counter:'0'
      }
    },
    methods:{
      playVideo(index){
        this.counter = index

        return this.counter
      }
    }
  }
</script>

<template>
  <section class="youtubeSection container">
    <div class="containerDisplay my-5 d-flex">

      <!-- Visione Grande dell'elemento selezionato su youtube -->
      <div class="bigView">
        <img :src="`/public/image${videoInfo[this.counter].src}`" class="w-100 imageVideo" alt="">
        <div class="youtubeChannel d-flex justify-content-center">
          <img :src="`/public/image/${videoInfo[this.counter].tv}.jpg`" alt="">
        </div>
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
          v-for="(card, index) in videoInfo"
          :key="card.id"
          class="video d-flex align-items-center"
          @click="playVideo(index)">
            <img :src="`/public/image${card.src}`" class="h-100 d-block" alt="">
            <span class="videoTextTitle">{{ card.title }} - {{ card.tv }}</span>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>

<style lang="scss">
  @use '../../scss/partials/youtubeSection.scss';
</style>