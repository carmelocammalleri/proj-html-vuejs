<script>
  export default{
    name: 'CardGallery',
    data(){
      return {
      }
    }
  }
</script>

<template>

  <section class="photoGallery py-4">
    <div class="container d-flex">
      <div class="left">
        <div class="card due mb-2">ciao</div>
        <div class="card due">ciao</div>
      </div>
      <div class="middle">
        <div class="card uno">ciao</div>
      </div>
      <div class="left">
        <div class="card due mb-2">ciao</div>
        <div class="card due">ciao</div>
      </div>

    </div>
  </section>





</template>

<style lang="scss">
  @use '../../scss/partials/cardGallery.scss';
</style>