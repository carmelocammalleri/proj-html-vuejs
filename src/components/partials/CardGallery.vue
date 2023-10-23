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
        <div class="card double mb-2">
          <img src="/public/image/photographers-mistakes.webp" alt="">
          <div class="btnInfo">
            <span class="mx-1">Travel</span>
            <span>Lifestyle</span>
          </div>
        </div>
        <div class="card double">
          <img src="/public/image/photographers-mistakes.webp" alt="">
          <div class="btnInfo">
            <span class="mx-1">Travel</span>
            <span>Lifestyle</span>
          </div>
        </div>
      </div>
      <div class="middle">
        <div class="card single">
          <img src="/public/image/best-places-300x200.webp" alt="">
          <div class="btnInfo">
            <span class="mx-1">Travel</span>
            <span class="mx-1">Lifestyle</span>
            <span class="mx-1">Food</span>
          </div>
        </div>
      </div>
      <div class="left">
        <div class="card double mb-2">
          <img src="/public/image/photographers-mistakes.webp" alt="">
          <div class="btnInfo">
            <span class="mx-1">Travel</span>
            <span>Lifestyle</span>
          </div>
        </div>
        <div class="card double">
          <img src="/public/image/photographers-mistakes.webp" alt="">
          <div class="btnInfo">
            <span class="mx-1">Travel</span>
            <span>Lifestyle</span>
          </div>
        </div>
      </div>

    </div>
  </section>

</template>

<style lang="scss">
  @use '../../scss/partials/cardGallery.scss';
</style>