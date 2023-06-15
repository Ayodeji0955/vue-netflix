<template>
    <div class="banner-comp ">
      
    </div>
  </template>
  
  
  <script setup lang="ts">
  // Imports
  
  
  </script>
  
  <style lang="scss" scoped>
  @import "@/sass/variable.scss";
  @import "@/sass/mixin.scss";
  
  .banner-comp { 
 
  
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
    