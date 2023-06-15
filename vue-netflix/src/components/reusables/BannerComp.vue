<template>
    <div class="banner-comp ">
        <div class="container banner-comp__container">
            <div class="row banner-comp__row row-cols-1 row-cols-md-3 justify-content-center">
                <div class="col-md-12 banner-comp__col">
                    <div class="row">
                        <div class="col-md-12">           
                            <h1 class="banner-comp__col--header"> 
                                <span class="banner-comp__col--sub-header">{{ props.first }}</span>
                            </h1>
                        </div>
                        <div class="col-md-12">
                            <p class="banner-comp__col--text">
                                <span class="banner-comp__col--sub-text">{{ props.third }}</span>
                                <span class="banner-comp__col--sub-text">{{ props.fourth }}</span>
                            </p> 

                        </div>
                        <div class="col banner-comp__cta">
                            <form class="row g-2 justify-content-center">
                                <div class="col-auto input-group-lg pt-2">
                                    <!-- <label for="inputPassword2" class="visually-hidden">{{ props.password }}</label> -->
                                    <input type="email" class="form-control banner-comp__sub-col--input" id="inputPassword2" placeholder="Email address" aria-describedby="inputGroup-sizing-lg">
                                </div>
                                <div class="col-auto pt-1">
                                    <button v-if="props.button" type="button"  class="banner-comp__cta--btn banner-comp__cta--button">
                                        {{ props.button }} <i class="fa-solid fa-greater-than"></i>
                                    </button>
                                </div>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </template>
  
  
  <script setup lang="ts">
  // Imports


   // Interface
   interface Props {
            // title: string,
            first: string,
            third: string,
            fourth: string,
            button ?: string,
        }

// Props
    const props = withDefaults(defineProps<Props>(), {
        // button: "none"
    })
  
  </script>
  
  <style lang="scss" scoped>
  @import "@/sass/variable.scss";
  @import "@/sass/mixin.scss";

  .banner-comp { 
    &__container {
        text-align: center;
        display: block;

    }

    &__col {
        // background-color: green; 
        display: flex;
        align-items: center;
        height: 70vh;

        &--header{
            padding-bottom: .5rem;
        }

        &--text{
            padding-bottom: 3rem;
        }

        &--sub-header { 
            font-size: $font-lg;
            font-weight: map-get($font-weights, bold);
            display: block;
            color: $color-light;
        }

        &--sub-text { 
            font-size: $font-rg;
            font-weight: map-get($font-weights, medium);
            display: block;
            color: $color-light;
        }
    }

    &__sub-col {

        &--input{
            background-color: transparent;
            transition: color 250ms cubic-bezier(0.5, 0, 0.1, 1) 0s;
            margin-top: 0.1rem;
            margin-bottom: 0.1rem;
            padding: 0.8rem 2.5rem;
            // padding-left:1rem;
            // padding-right:1rem;
            border: 0.5px solid white;
            font-weight:  map-get($font-weights, bold);
            box-shadow: 0px 0px 0px;
            border-radius: $radius-md;
        }
    }
  
    &__cta {
          
        @include cta;
      }
  }
  
  @media (min-width: 1024px) {
    .about {
        min-height: 100vh;
        display: flex;
        align-items: center;
    }
  }
  
  
  </style>
    