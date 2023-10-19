<script>
  export default {
    name: 'Footer'
  }
</script>

<template>
  <footer>
    <div class="footerWrapper container">

      <div class="upperFooter d-flex justify-content-between">
        <!-- DA CICLARE -->
        <div class="cardMenuInfo">
          <h5 class="titleMenu">ciao</h5>
          <ul class="menuInfo">
            <li>Resource</li>
            <li>Themes</li>
            <li>Belli</li>
            <li>Ciao</li>
          </ul>
        </div>

        <div class="cardMenuInfo">
          <h5 class="titleMenu">ciao</h5>
          <ul class="menuInfo">
            <li>Stories</li>
            <li>Themes</li>
            <li>Belli</li>
            <li>Ciao</li>
          </ul>
        </div>

        <div class="cardMenuInfo">
          <h5 class="titleMenu">ciao</h5>
          <ul class="menuInfo">
            <li>Stories</li>
            <li>Themes</li>
            <li>Belli</li>
            <li>Ciao</li>
          </ul>
        </div>

        <div class="cardMenuInfo">
          <h5 class="titleMenu">ciao</h5>
          <ul class="menuInfo">
            <li>Stories</li>
            <li>Themes</li>
            <li>Belli</li>
            <li>Ciao</li>
          </ul>
        </div>
        <!-- /DA CICLARE -->
    
        <div class="inputText d-flex flex-column">
          <h3> inserisci email</h3>
          <input type="text" placeholder="Email">
          <button class="btn btn-primary my-2" >Subscribe</button>
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