<script>
  export default {
    name: 'Header'
  }
</script>

<template>
  <header>
    <div class="newsUpdate">
      <div class="containerHead container d-flex justify-content-between">
        <div class="d-flex align-items-center">
          <div class="profileButton">
            <span class="buttonUpdates">NEWS UPDATES</span>
            <img class="profileImage" src="/image/ProfiloImage.jpg" alt="profilo">
          </div>
          <span> 05:52 the_</span>
        </div>
  
        <div class="socialHeader d-flex align-items-center">
          <div class="iconeArrow">
            &leftarrow; &rightarrow;
          </div>
          <div class="iconeSocial">
            icone
          </div>
        </div>
      </div>
    </div>

    <section class="banner container d-flex justify-content-between align-items-center ">
      <div class="containerBanner">
        <img id="logo" src="/public/image/anime-logo-300x89.webp" alt="logo-red">
      </div>

      <div >
        <img class="bannerImage" src="/public/image/header-banner.webp" alt="banner">
      </div>
    </section>

  </header>
</template>

<style lang="scss">
  @use '../scss/header.scss';
</style>