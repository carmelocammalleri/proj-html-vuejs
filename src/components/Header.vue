<script>
  export default {
    name: 'Header'
  }
</script>

<template>
  <header>
    <div class="newUpdate container d-flex justify-content-between">
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

    <section class="banner">
      <img src="/public/image/anime-whitelogo-300x89.png" alt="">
    </section>
  </header>
</template>

<style lang="scss">
  @use '../scss/header.scss';
</style>