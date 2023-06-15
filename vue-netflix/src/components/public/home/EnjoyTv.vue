<template>
    <div class="enjoy-tv">
        <div class="container">
            <div class="row justify-content-evenly">
                <div class="col-md-6 enjoy-tv__col align-self-center">
                    <h1 class="enjoy-tv__col--main-txt">Enjoy on your TV</h1>
                    <h2 class="enjoy-tv--col--sub-txt">
                        <span class="enjoy-tv__col--span">Watch on Smart TVs, Playstation, Xbox, Chromecast, </span>
                        <span class="enjoy-tv__col--span">Apple TV, Blu-ray players, and more.</span>
                    </h2>
                </div>
                <div class="col-md-4 enjoy-tv__col">
                    <img src="~@/assets/images/img_1/tv.png">
                </div>
            </div>
        </div>
        <hr class="enjoy-tv__hr">
    </div>
</template>


<script setup lang="ts">
// Imports components



</script>

<style lang="scss" scoped>
//imports from sass
  @import "@/sass/variable.scss";
  @import "@/sass/mixin.scss";

//styles
.enjoy-tv {
    background-color: $color-primary;
    padding-top: 4rem;

    &__col {

        &--main-txt {
            font-size: $font-lg;
            font-weight: map-get($font-weights, bold);
            color: $color-light;
            padding-bottom: 2rem;
        }

        
        &--span {
            font-size: $font-rg;
            font-weight: map-get($font-weights, regular);
            color: $color-light;
            display: block;
        }
    }

    &__hr {
        border: 5px solid grey;
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