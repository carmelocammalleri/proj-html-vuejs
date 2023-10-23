<script>
import {menuItems} from '../data/store.js'
  export default {
    name: 'Footer',
    data(){
      return {
        menuItems
      }
    }
  }
</script>

<template>
  <footer>
    <div class="footerWrapper container">

      <div class="upperFooter d-flex justify-content-between">
        <!-- DA CICLARE -->
        <div class="cardMenuInfo"
        v-for="(item, index) in menuItems"
        :key="index">
          <h5 class="titleMenu">{{item.title}}</h5>
          <ul class="menuInfo">
            <li v-for="i in item.element"><a href="#">{{ i }}</a></li>
          </ul>
        </div>
        <!-- /DA CICLARE -->
    
        <div class="inputText d-flex flex-column">
          <h3> inserisci email</h3>
          <input type="text" placeholder="Email">
          <button class="btn btn-tech my-2" >Subscribe</button>
        </div>
      </div>

      <div class="bottomFooter d-flex justify-content-between align-items-center">
          <img src="/public/image/anime-whitelogo-300x89.png" alt="">
          <span>Anime tech, theme qualcosa</span>
        </div>
        


    </div>
  </footer>
</template>

<style lang="scss">
  @use '../scss/footer.scss';
</style>