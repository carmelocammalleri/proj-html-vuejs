<script>
  export default {
    name: 'NavBar'
  }
</script>

<template>
  <nav class="containerNav">
    <div class="container d-flex justify-content-between align-items-center">
      <div>
        icon burger
      </div>
      <div class="menuHeader">
        <ul >
          <li>home</li>
          <li>lifestyle</li>
          <li>stories</li>
          <li>pages</li>
          <li>about us</li>
        </ul>
      </div>
      <div>
        search
      </div>
    </div>
  </nav>
</template>

<style lang="scss">
  @use '../../scss/partials/navBar.scss';
</style>