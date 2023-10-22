<script>
  export default {
    name: 'NavBar'
  }
</script>

<template>
  <nav class="containerNav">
    <div class="container d-flex justify-content-between align-items-center">
      <div>
        <i class="fa-solid fa-bars"></i>
      </div>
      <div class="menuHeader">
        <ul >
          <li>
            <i class="fa-solid fa-house mx-2"></i>
            <span>Home</span>
          </li>
          <li>
            <i class="fa-solid fa-suitcase mx-2"></i>
            <span>Lifestyle</span>
            <i class="fa-solid fa-chevron-down"></i>
          </li>
          <li>
            <i class="fa-solid fa-book-open-reader mx-2"></i>
            <span>Stories</span>
            <i class="fa-solid fa-chevron-down"></i>
          </li>
          <li>
            <i class="fa-solid fa-book mx-2"></i>
            <span>Pages</span>
            <i class="fa-solid fa-chevron-down"></i>
          </li>
          <li>
            <i class="fa-solid fa-user mx-2"></i>
            <span>About us</span>
          </li>
        </ul>
      </div>
      <div>
        <i class="fa-solid fa-magnifying-glass"></i>
      </div>
    </div>
  </nav>
</template>

<style lang="scss">
  @use '../../scss/partials/navBar.scss';
</style>