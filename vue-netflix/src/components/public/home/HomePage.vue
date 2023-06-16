<template>
    <div class="home-page">
        <NavBarVue
        />
        <BannerComp 
            first="Unlimited movies, TV shows, and more"
            third="Watch anywhere. Cancel anytime."
            fourth="We plug Individuals, Startups, SMEs and Higher Education"
            button="Get Started"
        />
    </div>
    <hr class="home-page__hr">
    <EnjoyTv/>
    <DownloadComp />
    <WatchComp />
</template>


<script setup lang="ts">
// Imports
import BannerComp from '../../reusables/BannerComp.vue';
import NavBarVue from './NavBar.vue';
import EnjoyTv from './EnjoyTv.vue';
import DownloadComp from './DownloadComp.vue';
import WatchComp from './WatchComp.vue';


</script>

<style lang="scss" scoped>

// .home-page {
//     position: relative;
// }
.home-page {
    background-image: 
        url('@/assets/images/img_1/overlay.png'),
        url('@/assets/images/img_1/bck.jpg');
    background-position:center;
    background-size:cover;
    height: 80vh;
    opacity: rgb(0 0 0 / 40%);

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