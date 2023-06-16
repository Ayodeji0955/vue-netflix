<template>
    <div class="download">
        <div class="container">
            <div class="row justify-content-between">
                <div class="col-md-4 download__col">
                    <img src="~@/assets/images/img_1/mobile.jpg">
                </div>
                <div class="col-md-6 download__col align-self-center">
                    <h1 class="download__col--main-txt">Download your shows to watch offline </h1>
                    <h2 class="download--col--sub-txt">
                        <span class="download__col--span">Save your favorites easily and always have something </span>
                        <span class="download__col--span">to watch.</span>
                    </h2>
                </div>
            </div>
        </div>
        <hr class="download__hr">
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
.download {
    background-color: $color-primary;
    padding-top: 4rem;

    &__col {

        &--main-txt {
            font-size: $font-lg;
            font-weight: map-get($font-weights, bold);
            color: $color-light;
            padding-bottom: 1rem;
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
        margin: 0 0;
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