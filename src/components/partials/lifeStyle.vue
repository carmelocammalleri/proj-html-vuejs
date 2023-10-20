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
          <div class="foto card">foto2</div>
          <div class="foto middle card">foto3</div>
          <div class="foto card">foto4</div>
        </div>
      </div>

    </div>
  </section>
</template>

<style lang="scss">
  @use '../../scss/partials/lifeStyle.scss';
</style>