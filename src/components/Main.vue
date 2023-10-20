<script>
import CardSlider from './partials/CardSlider.vue'
import CardGallery from './partials/CardGallery.vue'
import LifeStyle from './partials/lifeStyle.vue'
import FeaturedPosts from './partials/FeaturedPosts.vue'

  export default{
    name: 'Main',
    components:{
      CardSlider,
      CardGallery,
      LifeStyle,
      FeaturedPosts
    }
  }
</script>

<template>
  <main>
    <!-- slider -->
      <CardSlider/>
    <!-- slider -->

    <!-- photo gallery -->
      <CardGallery/>
    <!-- photo gallery -->

    <!-- lifestyle and stories -->
      <LifeStyle/>
    <!-- lifestyle and stories -->

    <!-- banner -->
    <section class="secbanner">

      <div class="banner container py-3" >
        <img class="bannerImage w-100" src="/public/image/header-banner.webp" alt="banner">
      </div>
    </section>
    <!-- banner -->

    <!-- feautured post -->
      <FeaturedPosts/>
    <!-- feautured post -->

    <!-- youtube -->
      
    <!-- youtube -->

    <!-- elementi e foto -->
    
    <!-- elementi e foto -->
  </main>
</template>

<style lang="scss" scoped>
@use '../scss/partials/variables' as *;
.secbanner{
  background-color: $bgColor;
  .bannerImage {
     border-radius: 5px;
    }
}
</style>
