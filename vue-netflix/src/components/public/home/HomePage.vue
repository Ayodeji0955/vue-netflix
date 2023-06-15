<template>
    <div class="home-page">
        <NavBarVue/>
    </div>
</template>


<script setup lang="ts">
// Imports
import NavBarVue from './NavBar.vue';


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
}

@media (min-width: 1024px) {
    .about {
        min-height: 100vh;
        display: flex;
        align-items: center;
    }
}
</style>