<template>
  <div id="app">
    <nav-bar></nav-bar>
    <image-carousel></image-carousel>
    <info-boxes></info-boxes>
    <MyFooter/>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import ImageCarousel from './components/ImageCarousel.vue';
import InfoBoxes from './components/InfoBoxes.vue';
import MyFooter from './components/MyFooter.vue';


export default {
  components: {
    NavBar,
    ImageCarousel,
    InfoBoxes,
    MyFooter
  }
}
</script>

<style>
/* Add global styles here */
</style>
