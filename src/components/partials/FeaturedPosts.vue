<script>
  export default {
    name: 'FeaturedPosts'
  }
</script>

<template>
  <section class="featuredPosts bg-white p-3">
    <div class="container">
        <h4>FEATURED POST</h4>
        <div class="cardSection d-flex justify-content-between">

          <div class="card m-1 p-5">
            <img class="card-img-top" src="`/public/image${card.src}`" alt="card.src">
            <div class="card-body text-center">
              <h6 class="card-title">card.title</h6>
              <p class="card-text">card.date</p>
            </div>
          </div>
          <div class="card m-1 p-5">
            <img class="card-img-top" src="`/public/image${card.src}`" alt="card.src">
            <div class="card-body text-center">
              <h6 class="card-title">card.title</h6>
              <p class="card-text">card.date</p>
            </div>
          </div>
          <div class="card m-1 p-5">
            <img class="card-img-top" src="`/public/image${card.src}`" alt="card.src">
            <div class="card-body text-center">
              <h6 class="card-title">card.title</h6>
              <p class="card-text">card.date</p>
            </div>
          </div>

        </div>
      </div>
    </section> 
</template>

<style lang="scss">

</style>
