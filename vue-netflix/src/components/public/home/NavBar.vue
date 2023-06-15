<template>
  <nav class="navbar bg-body-tertiary">
    <div class="container">
      <a class="navbar__favicon">
        <img class="navbar__favicon--img" src="~@/assets/images/img_1/favicon.png">
      </a>
      <div class="navbar__cta d-flex">
        <a href="/" class="navbar__cta--btn navbar__cta--button">Sign In</a>
      </div>
    </div>
  </nav>
</template>


<script setup lang="ts">
// Imports


</script>

<style lang="scss" scoped>
@import "@/sass/variable.scss";
@import "@/sass/mixin.scss";
.navbar { 
  padding-top: 1.5rem;

  &__favicon {
    
    &--img {
      width: 148px;

    }
  }

  &__cta {
        @include button;
    }
}

@media (min-width: 1024px) {
  .about {
      min-height: 100vh;
      display: flex;
      align-items: center;
  }
}

// rgb(0 0 0 / 40%);
</style>
  