<template>
  <div>
    <!--      <img src="@/assets/images/carusel/pexels-polina-tankilevitch-4110408.jpg">-->
    <b-carousel

        id="carousel-1"
        v-model="slide"
        :interval="1000"
        controls
        indicators
        class="carousel"

        @sliding-start="onSlideStart"
        @sliding-end="onSlideEnd"
    >
      <!--        style="text-shadow: 1px 1px 2px #333;"-->
      <!--        img-width="640"-->
      <!--        img-height="480"-->
      <b-carousel-slide
          caption="First slide"
          v-bind:img-src="img_all[2]"
      ></b-carousel-slide>
      <b-carousel-slide
          caption="Second Slide"
          v-bind:img-src="img_all[0]"
      ></b-carousel-slide>
      <b-carousel-slide
          caption="Third Slide"
          v-bind:img-src="img_all[1]"
      ></b-carousel-slide>
      <b-carousel-slide
          caption="Third Slide"
          v-bind:img-src="img_all[3]"
      ></b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script>

import img_1 from "@/assets/images/carusel/1.jpg"
import img_2 from "@/assets/images/carusel/2.jpg"
import img_3 from "@/assets/images/carusel/3.jpg"
import img_4 from "@/assets/images/carusel/4.jpg"


export default {
  name: "carusel-wine",
  data() {
    return {
      slide: 0,
      sliding: null,
      img_all: [
        img_1,
        img_2,
        img_3,
        img_4

      ]
    }
  },
  methods: {
    // onSlideStart(slide) {
    //   this.sliding = true
    // },
    // onSlideEnd(slide) {
    //   this.sliding = false
    // }
  }
}
</script>

<style scoped>
.carousel {
  width: 100%;
  height: 100%;
}
</style>