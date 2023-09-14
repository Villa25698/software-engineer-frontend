<template>
    <b-carousel
      controls
      indicators
      v-model="slide"
      :interval="4000"
      fade
      img-width="1024"
      img-height="480"
    >
      <b-carousel-slide
        v-for="(item, index) in items"
        :key="index"
        :img-src="item.img"
      >
        <h3>{{ item.text }}</h3>
      </b-carousel-slide>
    </b-carousel>
  </template>
  
  <script>
  export default {
    data() {
      return {
        slide: 0,
        items: [
          { img: 'path/to/image1.jpg', text: 'First slide' },
          { img: 'path/to/image2.jpg', text: 'Second slide' },
          // Add more items as needed
        ]
      }
    }
  }
  </script>
  