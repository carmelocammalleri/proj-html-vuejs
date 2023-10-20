<script>
  export default {
    name: 'lifeStyle'
  }
</script>

<template>
  <section class="lifeStyle py-5">
    <div class="container">
      <h4>Lifestyles & stories</h4>
      
      <div class=" presentation d-flex">
        <div class="card presentationPhotos">
          foto 1
        </div>
        <div class="listPhotos">
          
          <div class="foto">
            <div class="img">
              <img src="/public/image/healthy-foods.webp" alt="">
              <span>ciao belli del 93</span>
            </div>
          </div>
          <div class="foto middle">
            <div class="img">
              <img src="/public/image/healthy-foods.webp" alt="">
              <span>ciao belli del 93</span>
            </div>
          </div>
          <div class="foto">
            <div class="img">
              <img src="/public/image/healthy-foods.webp" alt="">
              <span>ciao belli del 93</span>
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