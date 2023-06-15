<template>
    <div class="home-page">
        <BannerView/>
    </div>
</template>


<script setup lang="ts">
// Imports
import BannerView from './BannerView.vue';

</script>

<style lang="scss" scoped>

.home-page {
    background-image: url('@/assets/images/img_1/bck.jpg');
    // background-color:aqua;
    background-position:center;
    background-size:cover;
    // padding-top: 7rem;
    height: 80vh;
}

// @media (min-width: 1024px) {
//     .about {
//         min-height: 100vh;
//         display: flex;
//         align-items: center;
//     }
// }
</style>